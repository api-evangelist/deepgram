# Deepgram (deepgram)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
