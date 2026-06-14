# Deepgram GraphQL Schema

This document describes the conceptual GraphQL schema for the Deepgram AI voice platform, covering speech-to-text transcription, text-to-speech synthesis, voice agent capabilities, audio intelligence analysis, and account management.

## Overview

Deepgram provides enterprise voice AI APIs including:

- **Speech-to-Text (STT)** — Pre-recorded and real-time streaming transcription via the Nova model family
- **Text-to-Speech (TTS)** — Natural speech synthesis via the Aura model family
- **Voice Agent API** — End-to-end conversational voice agent combining STT, LLM orchestration, and TTS
- **Audio Intelligence** — Sentiment analysis, summarization, topic detection, intent recognition, and entity extraction
- **Management API** — Project, API key, member, and usage administration

The schema below maps these capabilities into a GraphQL type system for exploratory and integration purposes.

## Schema Source

- Developer Portal: https://developers.deepgram.com/home
- API Reference: https://developers.deepgram.com/reference/deepgram-api-overview
- Speech-to-Text Docs: https://developers.deepgram.com/docs/stt/getting-started
- Text-to-Speech Docs: https://developers.deepgram.com/reference/text-to-speech-api/speak
- Audio Intelligence Docs: https://developers.deepgram.com/docs/audio-intelligence
- Voice Agent Docs: https://developers.deepgram.com/docs/voice-agent/getting-started
- GitHub: https://github.com/deepgram

## Root Types

### Query

The `Query` type exposes read operations for transcriptions, models, projects, API keys, members, and usage data.

### Mutation

The `Mutation` type exposes write operations for submitting transcription requests, synthesizing speech, managing projects, keys, and members.

### Subscription

The `Subscription` type supports real-time streaming for live transcription results and voice agent session events delivered over WebSocket.

## Type Categories

### Transcription Types

- `Transcription` — Top-level transcription job result containing metadata and channel results
- `TranscriptionDetails` — Detailed metadata for a transcription request including model, tier, and duration
- `TranscriptionStatus` — Enum of job states: QUEUED, PROCESSING, COMPLETED, FAILED
- `PrerecordedResult` — Full result for a pre-recorded audio transcription
- `StreamingResult` — Incremental result from a real-time streaming transcription session
- `Alternative` — One hypothesis for the transcript content (Deepgram returns the best alternative by default)
- `AlternativeDetails` — Confidence score and metadata for a transcript alternative
- `Word` — A single recognized word with timing and confidence data
- `WordDetails` — Extended metadata for a word including speaker tag and punctuation flag
- `WordConfidence` — Floating-point confidence score (0.0–1.0) for a word recognition
- `WordStart` — Start timestamp (in seconds) for a recognized word
- `WordEnd` — End timestamp (in seconds) for a recognized word
- `Paragraph` — A group of sentences identified by the smart formatting feature
- `ParagraphDetails` — Sentence count, speaker, and timing metadata for a paragraph
- `Sentence` — A single sentence within a paragraph
- `Utterance` — A contiguous speech segment attributed to a single speaker
- `UtteranceDetails` — Timing, confidence, and channel metadata for an utterance
- `UtteranceSpeaker` — Speaker identifier (integer) assigned during diarization

### Speaker and Channel Types

- `SpeakerDiarization` — Diarization result mapping speakers to utterances
- `Channel` — An audio channel in a multi-channel recording
- `ChannelDetails` — Index and search result metadata for a channel
- `ChannelResult` — Transcription alternatives for a specific channel

### Audio Types

- `Audio` — Reference to the audio source submitted for transcription
- `AudioDetails` — Format, sample rate, duration, and channel count metadata
- `AudioFormat` — Enum of supported container formats: MP3, WAV, FLAC, OGG, WEBM, MP4, M4A, AAC, OPUS
- `AudioSampleRate` — Integer sample rate in Hz (e.g. 8000, 16000, 44100, 48000)

### Language Types

- `Language` — A supported transcription language
- `LanguageCode` — BCP-47 language code string (e.g. "en-US", "es", "fr", "de", "ja")

### Feature Types

- `Feature` — A Deepgram transcription feature that can be enabled (e.g. diarize, punctuate, smart_format)
- `FeatureDetails` — Configuration parameters for an enabled feature
- `SmartFormat` — Smart formatting feature that formats numbers, dates, currencies, and more
- `Punctuate` — Feature that adds punctuation to the transcript
- `Numerals` — Feature that converts spoken numbers to numeric form
- `Profanity` — Profanity filter feature configuration
- `Redact` — PII redaction feature configuration (numbers, SSN, credit cards)
- `Keywords` — Keyword boosting feature to improve accuracy for domain-specific terms
- `Replace` — Term replacement feature to substitute words in the transcript
- `SearchTerm` — A term used in transcript search with timestamp and confidence results

### Audio Intelligence / NLP Types

- `NLP` — Container for all audio intelligence analysis results
- `Sentiment` — Overall or segment-level sentiment score and label
- `SentimentType` — Enum: POSITIVE, NEGATIVE, NEUTRAL, MIXED
- `Topic` — A detected topic with confidence score
- `Intent` — A detected user intent with confidence score
- `IntentDetails` — Input text segment and confidence for a detected intent
- `Entity` — A named entity extracted from the transcript
- `EntityType` — Enum: PERSON, ORGANIZATION, LOCATION, DATE, TIME, MONEY, QUANTITY, PRODUCT, EVENT, OTHER
- `EntityValue` — The raw text value of an extracted entity
- `Summary` — An abstractive or extractive summary of the transcript
- `SummaryType` — Enum: ABSTRACTIVE, EXTRACTIVE
- `Highlight` — A highlighted segment identified as significant
- `HighlightDetails` — Start/end timing and confidence for a highlight segment

### Voice Agent Types

- `Agent` — A configured voice agent session
- `AgentDetails` — Model, voice, LLM provider, and function configuration for an agent
- `AgentConfig` — Full configuration object for initializing a voice agent session

### Text-to-Speech Types

- `Voice` — An Aura TTS voice model available for speech synthesis
- `VoiceDetails` — Language, gender, accent, and latency characteristics for a voice
- `TextToSpeech` — A text-to-speech synthesis request
- `SpeechResult` — The synthesized audio result including format and byte length

### Management Types

- `APIKey` — A Deepgram API key with scopes, expiration, and project association
- `Token` — An authentication token with metadata
- `Error` — API error with code, message, and optional field-level details
- `Usage` — Aggregated usage metrics for a project
- `UsageDetails` — Breakdown of usage by model, feature, duration, and request count

## Authentication

All Deepgram API operations authenticate using API keys passed in the `Authorization` header as `Token <api_key>`. Scoped keys can be created for granular permission control.

## Real-Time Streaming

Live transcription and voice agent sessions use WebSocket connections. In GraphQL terms these map to `Subscription` operations delivering `StreamingResult` objects as audio frames arrive, with interim (is_final: false) and final (is_final: true) results.

## File Reference

- Schema: `deepgram-schema.graphql`
- APIs.yml: `../apis.yml`
