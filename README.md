# Deepgram (deepgram)

Deepgram is an enterprise voice AI platform that provides speech-to-text, text-to-speech, and voice agent APIs powered by advanced AI models. The platform offers real-time and batch transcription through its Nova model family, natural-sounding speech synthesis through its Aura model family, and an end-to-end Voice Agent API that combines STT, LLM orchestration, and TTS into a single real-time interface.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Artificial Intelligence
- Speech-To-Text
- Text-To-Speech
- Transcription
- Voice AI

## Timestamps

- **Created:** 2026-03-20
- **Modified:** 2026-05-19

## APIs

### Deepgram Speech-To-Text API

The Deepgram Speech-to-Text API provides accurate, fast transcription of audio content using advanced AI models. It supports both pre-recorded audio files and real-time streaming audio, delivering transcripts in under 300 milliseconds. The API includes features such as punctuation, diarization, language detection, smart formatting, and support for multiple languages and audio formats.

- **Human URL:** [https://developers.deepgram.com/docs/stt/getting-started](https://developers.deepgram.com/docs/stt/getting-started)
- **Base URL:** `https://api.deepgram.com`

#### Tags

- Audio
- Speech Recognition
- Speech-To-Text
- Transcription

#### Properties

- [Documentation](https://developers.deepgram.com/docs/stt/getting-started)
- [OpenAPI](openapi/deepgram-speech-to-text-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/deepgram-speech-to-text.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deepgram-speech-to-text.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/deepgram-speech-to-text-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Rules](rules/deepgram-speech-to-text-api-rules.yml)
- [Capabilities](capabilities/deepgram-speech-to-text-api-capabilities.yml)

### Deepgram Text-To-Speech API

The Deepgram Text-to-Speech API converts text into natural-sounding speech using the Aura model family. It supports both single text requests and continuous streaming text-to-speech, delivering sub-200 millisecond latency suitable for real-time voice agents and conversational AI applications. The API offers multiple voice options and is designed for enterprise-grade deployments including voicebots, IVR systems, and interactive voice applications.

- **Human URL:** [https://developers.deepgram.com/reference/text-to-speech-api/speak](https://developers.deepgram.com/reference/text-to-speech-api/speak)
- **Base URL:** `https://api.deepgram.com`

#### Tags

- Audio
- Speech Synthesis
- Text-To-Speech
- Voice

#### Properties

- [Documentation](https://developers.deepgram.com/reference/text-to-speech-api/speak)
- [OpenAPI](openapi/deepgram-text-to-speech-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/deepgram-text-to-speech.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deepgram-text-to-speech.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/deepgram-text-to-speech-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Rules](rules/deepgram-text-to-speech-api-rules.yml)
- [Capabilities](capabilities/deepgram-text-to-speech-api-capabilities.yml)

### Deepgram Voice Agent API

The Deepgram Voice Agent API is an end-to-end solution that combines speech-to-text, LLM orchestration, and text-to-speech into a single real-time API. It simplifies the development of conversational voice agents by eliminating the need to stitch together multiple services. The API includes built-in barge-in detection, turn-taking prediction, function calling, and mid-session control to ensure smooth, natural conversations without pauses or interruptions.

- **Human URL:** [https://deepgram.com/product/voice-agent-api](https://deepgram.com/product/voice-agent-api)
- **Base URL:** `https://api.deepgram.com`

#### Tags

- Conversational AI
- Real-Time
- Voice Agent
- Voice AI

#### Properties

- [Documentation](https://developers.deepgram.com/docs/voice-agent/getting-started)
- [AsyncAPI](asyncapi/deepgram-voice-agent-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/deepgram-management.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deepgram-management.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/deepgram-speech-to-text.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deepgram-speech-to-text.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/deepgram-text-to-speech.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deepgram-text-to-speech.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Deepgram Audio Intelligence API

The Deepgram Audio Intelligence API provides advanced analysis capabilities for audio and text content. It offers features including sentiment analysis, summarization, topic detection, and intent recognition. These capabilities allow developers to extract structured insights from transcribed audio or text input, enabling use cases such as call center analytics, meeting summarization, and content categorization.

- **Human URL:** [https://developers.deepgram.com/docs/audio-intelligence](https://developers.deepgram.com/docs/audio-intelligence)
- **Base URL:** `https://api.deepgram.com`

#### Tags

- Audio Intelligence
- Sentiment Analysis
- Summarization
- Topic Detection

#### Properties

- [Documentation](https://developers.deepgram.com/docs/audio-intelligence)
- [OpenAPI](openapi/deepgram-speech-to-text-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/deepgram-speech-to-text.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deepgram-speech-to-text.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Deepgram Management API

The Deepgram Management API allows developers to programmatically manage their Deepgram account resources. It provides endpoints for creating and managing API keys, configuring projects, managing team members, and monitoring usage. This API enables automation of administrative tasks and integration of Deepgram account management into existing workflows and infrastructure tooling.

- **Human URL:** [https://developers.deepgram.com/docs/create-additional-api-keys](https://developers.deepgram.com/docs/create-additional-api-keys)
- **Base URL:** `https://api.deepgram.com`

#### Tags

- Administration
- API Keys
- Management
- Projects

#### Properties

- [Documentation](https://developers.deepgram.com/docs/create-additional-api-keys)
- [OpenAPI](openapi/deepgram-management-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/deepgram-management.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deepgram-management.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Rules](rules/deepgram-management-api-rules.yml)
- [Capabilities](capabilities/deepgram-management-api-capabilities.yml)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [LinkedIn](https://www.linkedin.com/company/deepgram)
- [Documentation](https://developers.deepgram.com/home)
- [Documentation](https://developers.deepgram.com/reference/deepgram-api-overview)
- [Pricing](https://deepgram.com/pricing)
- [Authentication](https://developers.deepgram.com/docs/authenticating)
- [Changelog](https://developers.deepgram.com/changelog)
- [SDK](https://github.com/deepgram/deepgram-python-sdk)
- [SDK](https://github.com/deepgram/deepgram-js-sdk)
- [Website](https://deepgram.com/)
- [Privacy Policy](https://deepgram.com/privacy)
- [Terms of Service](https://deepgram.com/tos)
- [JSON-LD](json-ld/deepgram-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/deepgram-transcript-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Vocabulary](vocabulary/deepgram-vocabulary.yml)
- [Features](undefined)
- [Integrations](https://deepgram.com/partners)
- [L L Ms Txt](https://deepgram.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
