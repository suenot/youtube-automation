# youtube-automation

YouTube-specific automation is grouped here as two pinned Git submodules:

| Component | Purpose |
| --- | --- |
| [`youtube-automation-metadata`](https://github.com/suenot/youtube-automation-metadata) | Prepare YouTube titles, descriptions, tags, chapters, and subtitles. |
| [`youtube-automation-prepare`](https://github.com/suenot/youtube-automation-prepare) | Upload a prepared video and metadata through YouTube Studio. |

Clone with `git clone --recurse-submodules git@gitlab.com:reforms-lab/youtube-automation.git`, or run `git submodule update --init --recursive` after cloning. The two tools retain their own commands and dependencies; this repository pins compatible revisions and documents their relationship. Other social publishers remain separate projects in `root`.

The public GitHub repositories are the canonical submodule URLs. Private copies under `reforms-lab` on GitLab use the same commit history.

Version: see `VERSION`. Changes to this aggregator are recorded in `CHANGELOG.md`.
