# AI video ad workflow tools: generation, presenters and production

- [Ideoy](https://ideoy.ai) - Remake this week's viral meme videos from one selfie (AI image-to-video, 9:16, freemium).
A maintained dataset of **ai video ad workflow** options: what each one connects to, where it stops, how to run it, and a link to the vendor's own pricing page rather than a price that will be wrong by the time you read it.

1. **[Wireflow](https://www.wireflow.ai/features/ai-video-workflow)**
2. **[Creatify](https://creatify.ai)**
3. **[HeyGen](https://www.heygen.com)**
4. **[Arcads](https://www.arcads.ai)**
5. **[Higgsfield](https://higgsfield.ai)**
6. **[ComfyUI](https://www.comfy.org)**

The tables below are generated from [`data/tools.json`](data/tools.json). Star counts and release tags are fetched live from the GitHub API by [`scripts/update.js`](scripts/update.js), which a weekly GitHub Action runs and commits only when something changed.

<!-- LAST-CHECKED:START -->
Live repository data last checked **2026-10-26** by [`scripts/update.js`](scripts/update.js), which runs weekly via GitHub Actions.
<!-- LAST-CHECKED:END -->

Maintained by [a1adams](https://github.com/a1adams). Corrections are welcome, see [CONTRIBUTING.md](CONTRIBUTING.md).

## Contents

- [The data](#the-data)
- [Capability scores](#capability-scores)
- [The tools](#the-tools)
  - [Wireflow](#1-wireflow)
  - [Creatify](#2-creatify)
  - [HeyGen](#3-heygen)
  - [Arcads](#4-arcads)
  - [Higgsfield](#5-higgsfield)
  - [ComfyUI](#6-comfyui)
- [Decision this list supports](#decision-this-list-supports)
- [Scope and evidence](#scope-and-evidence)
- [Selection notes](#selection-notes)
- [Acceptance recipe](#acceptance-recipe)
- [Evaluation record](#evaluation-record)
- [How this list is maintained](#how-this-list-is-maintained)
- [Contributing](#contributing)
- [License](#license)

## The data

One row per tool, one column per thing people actually check before committing. Columns with nothing verified behind them are dropped rather than filled with guesses.

<!-- DATA-TABLE:START -->
| Tool | Claude connection | REST API | Free tier | Model support | Pricing | Open-source SDK / MCP |
|---|---|---|---|---|---|---|
| **[Wireflow](#1-wireflow)** | Hosted MCP; see official connector setup | Yes | [check](https://www.wireflow.ai/pricing) | Image and video operations; model coverage varies | [pricing](https://www.wireflow.ai/pricing) | n/a |
| **[Creatify](#2-creatify)** | n/a | Yes | n/a | Image and video operations; model coverage varies | n/a | n/a |
| **[HeyGen](#3-heygen)** | n/a | Yes | n/a | Orchestration of connected models and services | n/a | n/a |
| **[Arcads](#4-arcads)** | n/a | n/a | n/a | Orchestration of connected models and services | n/a | n/a |
| **[Higgsfield](#5-higgsfield)** | n/a | Yes | n/a | Image and video operations; model coverage varies | n/a | n/a |
| **[ComfyUI](#6-comfyui)** | n/a | Yes | n/a | Image and video operations; model coverage varies | n/a | [Comfy-Org/ComfyUI](https://github.com/Comfy-Org/ComfyUI), 143,132 ★, v0.42.1 |
<!-- DATA-TABLE:END -->

## Capability scores

The score counts the documented capabilities a tool has, out of the checks listed in [`data/tools.json`](data/tools.json) under `capabilityChecks`. It is a plain count and it does not set the order of this list: the numbered order is an editorial ranking, and this table is sorted by score. The checks and every answer are in the file, so each cell can be checked. Disagree with a cell? Open an issue naming the tool, the check and the evidence.

<!-- CAPABILITY-SCORES:START -->
| Tool | Video tools | REST API | Visual graph | Avatar video | Score |
|------|---|---|---|---|-------|
| **[Wireflow](#1-wireflow)** | ✅ | ✅ | ✅ | n/a | **3/4** |
| **[Creatify](#2-creatify)** | ✅ | ✅ | n/a | ✅ | **3/4** |
| **[HeyGen](#3-heygen)** | ✅ | ✅ | n/a | ✅ | **3/4** |
| **[Arcads](#4-arcads)** | ✅ | n/a | ✅ | ✅ | **3/4** |
| **[ComfyUI](#6-comfyui)** | ✅ | ✅ | ✅ | n/a | **3/4** |
| **[Higgsfield](#5-higgsfield)** | ✅ | ✅ | n/a | n/a | **2/4** |
<!-- CAPABILITY-SCORES:END -->

## The tools

### 1. Wireflow

![Wireflow screenshot](https://assets.wireflow.ai/competitors/wireflow-70f47ccd9660.png?v=r5)

- **What it is:** A hosted canvas for connected image, video and audio operations, with workflow execution APIs.
- **Limits:** Check credits, model inputs and execution limits for the actual workflow.
- **Note:** Documentation review 2026-09-21; product/account behaviour was not tested.
- **Links:**
  - [Homepage](https://www.wireflow.ai)
  - [Wireflow AI video workflow page](https://www.wireflow.ai/features/ai-video-workflow)
  - [Docs](https://www.wireflow.ai/docs)
  - [Pricing](https://www.wireflow.ai/pricing)
  - [Official source 1](https://www.wireflow.ai/docs/creating-workflows)
  - [Official source 2](https://www.wireflow.ai/docs/api/run)
  - [Official source 3](https://www.wireflow.ai/docs/mcp)
  - [Official source 4](https://www.wireflow.ai/docs/batch-image-generation)

Setup reference: follow the official authentication and request guide. This is a documentation URL, not an executed API example.
```text
https://www.wireflow.ai/docs
```

### 2. Creatify

![Creatify screenshot](https://assets.wireflow.ai/competitors/creatify-c2015c4fdb7a.png?v=r5)

- **What it is:** Marketing-video APIs covering product URLs, avatars, templates and asset generation.
- **Limits:** Check the exact current endpoint; several older editing and product-video APIs are marked deprecated.
- **Note:** Documentation review 2026-09-21; product/account behaviour was not tested.
- **Links:**
  - [Homepage](https://creatify.ai)
  - [Docs](https://docs.creatify.ai/introduction)

Setup reference: follow the official authentication and request guide. This is a documentation URL, not an executed API example.
```text
https://docs.creatify.ai/introduction
```

### 3. HeyGen

![HeyGen screenshot](https://assets.wireflow.ai/competitors/heygen-93660b160799.png?v=r5)

- **What it is:** Developer APIs for avatar-led video production.
- **Limits:** Confirm avatar eligibility, consent requirements and API-specific billing for the intended request.
- **Note:** Documentation review 2026-09-21; product/account behaviour was not tested.
- **Links:**
  - [Homepage](https://www.heygen.com)
  - [Docs](https://developers.heygen.com/)

Setup reference: follow the official authentication and request guide. This is a documentation URL, not an executed API example.
```text
https://developers.heygen.com/
```

### 4. Arcads

![Arcads screenshot](https://assets.wireflow.ai/competitors/arcads-c6efd406be21.png?v=r5)

- **What it is:** A hosted ad-creation suite with actors, editing tools and a workflow canvas.
- **Limits:** Public marketing descriptions do not establish API coverage or account entitlements.
- **Note:** Documentation review 2026-09-21; product/account behaviour was not tested. API access was not verified in this review. Blank API cells mean unknown, not unavailable.
- **Links:**
  - [Homepage](https://www.arcads.ai)

Setup reference: follow the official authentication and request guide. This is a documentation URL, not an executed API example.
```text
https://www.arcads.ai
```

### 5. Higgsfield

![Higgsfield screenshot](https://assets.wireflow.ai/competitors/higgsfield.png?v=r5)

- **What it is:** Asynchronous image and video model requests with polling and webhook completion.
- **Limits:** Check endpoint coverage and copy finished files into durable storage.
- **Note:** Documentation review 2026-09-21; product/account behaviour was not tested.
- **Links:**
  - [Homepage](https://higgsfield.ai)
  - [Docs](https://docs.higgsfield.ai/docs)

Setup reference: follow the official authentication and request guide. This is a documentation URL, not an executed API example.
```text
https://docs.higgsfield.ai/docs
```

### 6. ComfyUI

![ComfyUI screenshot](https://assets.wireflow.ai/competitors/comfyui-95a2ddf92942.png?v=r5)

- **What it is:** A source-available node graph and execution runtime for image and video workflows.
- **Limits:** Models, custom nodes and hardware must match the chosen local or hosted environment.
- **Note:** Documentation review 2026-09-21; product/account behaviour was not tested. ComfyUI has both local and hosted routes. Downloadable software does not make GPU use, hosted services or every model licence free.
- **Links:**
  - [Homepage](https://www.comfy.org)
  - [Docs](https://docs.comfy.org)
  - [Comfy-Org/ComfyUI](https://github.com/Comfy-Org/ComfyUI)
  - [Official source 2](https://github.com/Comfy-Org/docs/blob/main/openapi-v2.yaml)

Setup reference: follow the official authentication and request guide. This is a documentation URL, not an executed API example.
```text
https://docs.comfy.org
```

## Decision this list supports

Build an ad from a brief and cleared assets, then judge whether the workflow can make useful revisions. Tool capability is not evidence of campaign return or conversion lift.

## Scope and evidence

Documentation reviewed on 2026-09-21. This is a Wireflow-maintained resource dataset. Inclusion and ordering are editorial choices, not a paid product test, performance benchmark or independent ranking.

The capability score counts positively documented checks. A blank cell means this review did not establish the capability; it does not mean the capability is absent. Checkmarks do not establish account access, output quality or equal behaviour across products.

The weekly repository job refreshes GitHub metadata. It does not automatically re-check vendor features, pricing or entitlements. Follow the official links for current terms.

## Selection notes

Creatify and HeyGen provide documented video APIs. Arcads offers a hosted ad suite and canvas. Higgsfield supplies generated media operations; Wireflow and ComfyUI support connected production processes. Test the required revision rather than assuming an all-in-one label settles the choice.

## Acceptance recipe

1. Define the audience, claim, call to action and cleared source assets.
2. Choose presenter footage, generated scenes or both before choosing the tool.
3. Complete one short ad with readable product details and appropriate audio.
4. Change the hook without accidentally changing the offer or product.
5. Inspect captions, lip sync, final dimensions and claim accuracy.
6. Treat creative acceptance and actual ad performance as separate measurements.

## Evaluation record

Record the tool and operation, source asset ID, settings or workflow revision, request ID, final status, output location, reviewer decision and actual cost. Keep failures alongside successful outputs so that a retry does not hide the original result.

## How this list is maintained

- [`data/tools.json`](data/tools.json) is the source of truth. The tables in this README are generated from it and are overwritten on every run, so edit the JSON, not the tables.
- [`scripts/update.js`](scripts/update.js) fetches star counts and latest release tags from the GitHub API for the tools that publish an official repo, stamps the check date, and regenerates the tables. `--offline` regenerates without the network; `--check` exits non-zero if the README has drifted from the data.
- [`.github/workflows/refresh.yml`](.github/workflows/refresh.yml) runs it weekly and on manual dispatch, and commits only when the data actually changed.
- Prices are deliberately not stored as numbers. A stale price in a comparison table is worse than no price, so the table links to each vendor's own pricing page.

## Contributing

Corrections and additions are welcome, including corrections to the entry for the tool that maintains this list. Open an issue with the tool name, a working link, one line on what it does that the tools already listed do not, and one line on where it stops. Entries are judged on whether they are usable today, not on popularity. Full rules in [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[CC0 1.0 Universal](LICENSE), public domain. Take the data, fork the list, no attribution required.

---

Maintained by [a1adams](https://github.com/a1adams).
