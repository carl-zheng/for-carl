# KreadoAI integration

This directory binds the platform-neutral production handoff to KreadoAI's HTTP MCP service without storing credentials.

## Current state

- Connection: `AUTHENTICATED_READ_ONLY_VERIFIED`
- Endpoint reachability: `VERIFIED` by an unauthenticated HTTP `HEAD` request on 2026-08-23
- Authenticated MCP initialization and the initial read-only tool call: `VERIFIED` on 2026-08-23
- Local personal plugin: authenticated and verified; three Seedance submission schemas and one polling schema are loaded under prompt approval
- First paid product-consistency test: task `192751` succeeded on 2026-08-23 using `Doubao-seedance-mini-2`, 720P, 9:16, four seconds, silent audio, and one output
- Visual QA: `CONDITIONAL_PASS_PACKAGING_HERO_ONLY`; the package remained stable, but the partial figure subset must not be used as proof of the full 24-piece lineup
- Further generation: not authorized; the one-task approval was consumed and cannot authorize a retry or another submission
- Secret environment variable: `KREADOAI_API_TOKEN`
- Repository-stored credentials: prohibited

The local plugin reads the custom `apiToken` header from `KREADOAI_API_TOKEN`. Do not paste the key into the plugin, this repository, logs, prompts, or generated artifacts.

## Safe connection test — completed

The initial allowlist exposes only `list_seedance_builtin_virtual_character_labels`. On 2026-08-23, KreadoAI successfully returned its built-in nationality, profession, and gender label tree. The test did not create a media task or request private account information, and the credential was not logged or persisted.

Do not submit another video, crawl a page, upload or delete assets, synthesize speech, or retry task `192751` without a fresh named approval. Every media submission remains approval-gated, and the supplied documentation does not identify the unit represented by `taskAmount`; task `192751` returned `24.00`, whose currency or credit unit must not be inferred.

## Generation schema discovery — completed

The plugin exposes `submit_seedance_text_to_video`, `submit_seedance_video_with_references`, `submit_seedance_first_last_video`, and `batch_get_video_generation_detail`. On 2026-08-23, their live declarations were read without invoking any submission tool. Exact field names, public-URL media inputs, reference indexing, duration, model, resolution, ratio, audio, generation-count, web-search, and polling parameters are now mapped. The default approval mode remains `prompt`, generation count remains capped at one until separately approved, and deletion stays disabled.

## Production binding

After verification, map neutral production jobs by capability:

- no reference → `submit_seedance_text_to_video`
- image, video, or audio references → `submit_seedance_video_with_references`
- approved first and last frames → `submit_seedance_first_last_video`

The current three-second opening job is shorter than Seedance's documented four-second minimum, so generate at least four seconds and trim during editing, or obtain approval to regroup it. Keep exact commercial text and subtitles editor-owned. The successful Mini/720P test validates the connection and packaging-hero route only; production model, resolution, ratio, audio behavior, and every next payload still require explicit selection and approval.
