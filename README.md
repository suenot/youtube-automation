# youtube-automation

YouTube-specific automation is grouped here as two pinned Git submodules:

| Component | Purpose |
| --- | --- |
| [`youtube-automation-metadata`](https://github.com/suenot/youtube-automation-metadata) | Prepare YouTube titles, descriptions, tags, chapters, and subtitles. |
| [`youtube-automation-prepare`](https://github.com/suenot/youtube-automation-prepare) | Upload a prepared video and metadata through YouTube Studio. |

Clone with `git clone --recurse-submodules git@gitlab.com:reforms-lab/youtube-automation.git`, or run `git submodule update --init --recursive` after cloning. The two tools retain their own commands and dependencies; this repository pins compatible revisions and documents their relationship. Other social publishers remain separate projects in `root`.

The public GitHub repositories are the canonical submodule URLs. Private copies under `reforms-lab` on GitLab use the same commit history.

## Caribbean Awesome publication

The first Short is [publicly listed on the channel](https://www.youtube.com/@caribbeanawesome/shorts) at [wZqnYESB3Us](https://www.youtube.com/shorts/wZqnYESB3Us). The verified channel ID is `UCa5ng53XBSQ6Z-kZ0u4uFdQ`, display name **Caribbean Awesome**. The publisher imported the authorized Firefox session into its own persistent Camoufox profile and passed a read-only preflight against this exact Short: channel, saved title, description and Public visibility matched. It did not attach a file or press Save/Publish. The publisher's `--request-id` journal and `--require-public` guard support repeatable future calls; use explicit `--visibility public` for this campaign. See [publisher instructions](youtube-automation-prepare/README.md) for the command and recovery rules.

Version: see `VERSION`. Changes to this aggregator are recorded in `CHANGELOG.md`.

If the saved session expires, refresh it with the publisher's
`login.py --refresh --firefox-profile '/path/to/profile' --channel-handle @caribbeanawesome`.
Refresh keeps the existing channel binding and request journal, verifies the
same channel, and restores previous cookies if verification fails. This repair
is covered by 14 focused login/channel checks. On 2026-10-08, live refresh verified
the saved channel and the CLI published the [Key West Short](https://www.youtube.com/shorts/F4gRxvE5MX0)
with matching saved metadata and Public visibility. A cookie-free Camoufox session
confirmed its exact title, channel and 41.721-second playback.
