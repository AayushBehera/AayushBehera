# Profile asset specification

This repository's profile README uses a shared vector system rather than unrelated badges or third-party stat cards.

## Layout measurements

| Asset | Native size | Aspect ratio | Intended placement | Notes |
|---|---:|---:|---|---|
| `assets/profile/cover.svg` | 1400 × 460 | 3.043:1 | Full-width hero | 60 px left inset; right-side system panel; static vector artwork |
| `assets/profile/capabilities.svg` | 1200 × 350 | 3.429:1 | Full-width capability map | Four equal capability cards with 18 px outer card corner radius |
| Project SVGs | 960 × 540 | 16:9 | Two-column project table | Consistent title baseline, left accent rail, inner frame, 22 px outer inset |

### Project artwork

- `projects/changeguard.svg` — supported artifact inputs, shared analysis stages, advisory report.
- `projects/adbibe-reporting.svg` — advertising channels, normalized data layer, Gemini-assisted analytics and report workflow. Development caveats are shown in the art.
- `projects/sensorspine.svg` — synthetic transaction inputs and real contextual sources, forecasting, surplus classification, recommendations, outcome feedback.
- `projects/self-healing-sdn.svg` — Ryu/PPO control loop, OpenFlow 1.3 topology, failed link and alternate route.
- `projects/phishing-forensics.svg` — Gmail page, Manifest V3 extension, Express/Gemini analysis and Next.js SOC dashboard.
- `projects/error-mechanism.svg` — stack-trace input, deterministic TypeScript rules, diagnosis output and local history.

All project SVGs are **system diagrams**, not screenshots of running software. No demo endpoint is shown unless a public deployment URL can be verified. Existing placeholder screenshot links in project documentation were not reused as if they were current captures.

## Visual tokens

| Token | Value | Usage |
|---|---|---|
| Ink | `#0A1020` | Primary background |
| Deep surface | `#121D30` | Panels |
| Elevated surface | `#19213B` | Secondary panels |
| Primary violet | `#C4B5FD` / `#7C3AED` | Identity and DevOps |
| Cyan | `#A5F3FC` / `#0891B2` | Services and data |
| Mint | `#BBF7D0` / `#16A34A` | Data pipeline / successful paths |
| Coral | `#FECDD3` / `#E11D48` | Network failure and alerts |
| Amber | `#FDE68A` / `#D97706` | Warnings and caveats |
| Main text | `#F8FAFC` | Headlines |
| Muted text | `#A9B7CC` | Supporting labels |

## Typography and spacing

- Font stack: `Inter, Segoe UI, Arial, sans-serif`; code labels use a monospace stack.
- The base spacing rhythm is 8 px.
- Cover: 60 px left title inset; key title at y=165; role line at y=209; supporting line at y=254.
- Project panels: outer border inset 22 px; content inset 54 px; title baseline y=101; section labels at y=59; content begins at y=165; consistent footer at y=484.
- Images use fixed SVG `viewBox` values and preserve aspect ratio when rendered with `width="100%"`.

## Accessibility and rendering

- All SVGs are static; no flashing, animation, external fonts, or JavaScript.
- Every embedded image in the README has descriptive alt text.
- Color is paired with labels and text, rather than being the only way to read a status.
- Diagrams are vector assets and scale without raster blur.
- The README is Markdown-first; GitHub does not provide arbitrary custom CSS or interactive controls inside profile READMEs.

## Accuracy rules

- SensorSpine operational transactions are explicitly synthetic until a live POS feed is connected; its HCES, ERA5, and holiday context is distinct.
- Adbibe's repository documentation describes mock development data and mock integration adapters; real OAuth flows and outbound report delivery remain follow-up work.
- ChangeGuard is advisory; human review remains in the deployment decision.
- Self-Healing SDN Phase 1 is complete; Phase 2 is planned.
- Error Mechanism uses 18 deterministic rules; its heuristic score is not a calibrated probability.
- The two claude-mem pull requests shown in the README are merged. The two Aider pull requests are open and are labelled as under review.
- Dates, job impact numbers, GitHub contribution counts, and live demo URLs are not invented.
