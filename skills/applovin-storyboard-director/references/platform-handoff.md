# Platform-Neutral Production Handoff

Use this contract to keep the approved creative independent from the user's eventual video-production platform.

## Binding states

- `PENDING_USER_PLATFORM`: provider and capabilities are not supplied; produce a complete neutral handoff.
- `PROFILE_INCOMPLETE`: provider is named but one or more capabilities materially affect job decomposition.
- `PROFILE_VERIFIED`: current platform documentation or user-approved configuration supplies the required capabilities.

Never infer a platform profile from general market knowledge. Do not place credentials, tokens, cookies, or private endpoints in repository artifacts.

## Production handoff structure

`production-handoff-v1.json` should contain:

1. **Source lock**
   - storyboard and script IDs and versions
   - approved duration, market, language, concept, and dominant memory

2. **Platform binding**
   - status
   - provider and adapter ID, or `null`
   - profile version and verification source, or `null`

3. **Global delivery requirements**
   - aspect ratio, resolution, frame rate, audio, caption, and file format when verified; otherwise `UNBOUND`
   - product-identity and visual-style continuity locks

4. **Asset manifest**
   - stable asset IDs, origin, availability, role, and whether upload or remote reference will be required

5. **Provider-neutral job units**
   - job ID and shot IDs
   - duration required
   - source asset IDs
   - capability needs such as text-to-video, still-to-motion, multi-reference consistency, compositing, background generation, lip sync, or audio generation
   - expected output role
   - no provider prompt syntax or API payload

6. **Editor-owned layers**
   - exact on-screen text, price, policy, logo, subtitles, music, sound effects, and CTA overlays that should remain outside generative media unless a verified workflow says otherwise

7. **Validation rules**
   - timeline duration
   - shot coverage
   - product-identity continuity
   - claim and offer consistency
   - launch-time dynamic-value checks

## Minimum platform profile for later binding

Collect only the fields that affect execution:

- provider and connection mode: API, browser workflow, upload/export, or local tool
- accepted source media and per-job reference limits
- available generation modes and identity/reference controls
- minimum and maximum clip duration
- supported aspect ratios, resolutions, frame rates, and output containers
- whether audio, speech, lip sync, captions, logos, and exact text are supported or should remain editor-owned
- job concurrency, queue/status behavior, retry rules, and output retrieval
- any required platform-specific fields, limits, or cost controls

After the profile is verified, a downstream Video Producer or platform adapter may translate neutral job units into provider prompts and requests. That translation must not change the storyboard, approved copy, claims, offer, or timing without an explicit upstream revision.

