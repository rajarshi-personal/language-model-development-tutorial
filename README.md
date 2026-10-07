# Model Workshop

A single-page, offline interactive tutorial for Python and Java developers:
build a knowledge-base assistant, fine-tune a small language model, evaluate
it, and deploy it with Ollama or Hugging Face.

**Open `index.html` in your browser.** No build, server, installation or internet
connection is needed to use the tutorial. The page defaults to a light theme
and includes a dark-theme toggle.

The **Project kit** button downloads a ZIP containing 22 embedded project files:
sample-data generation, retrieval, LoRA training, model merging, Ollama export,
Python/Java inference, a Gradio app, evaluation, and setup instructions.
Running those examples requires their documented dependencies and initial model
downloads. The HTML does not run or train a language model in the browser.

## License and third-party rights

Copyright (c) 2026 Rajarshi Ray — rajarshir@gmail.com.

The original project materials are **source-available, free to use, with
redistribution restricted** under [LICENSE](LICENSE). You may read, download,
run and modify them for personal, educational and internal business use.
Public redistribution, mirroring, rehosting and distribution of modified
copies require prior written permission, subject to the license's exceptions.
Sharing a link to the official tutorial is allowed.

This is a custom source-available license, not an OSI open-source license:
the [Open Source Definition](https://opensource.org/osd) requires redistribution
rights. The restriction expresses the owner's licensing preference; it is not
a technical mechanism that prevents copying a public website.

Third-party libraries, dependencies, tools, models and other third-party
materials retain their respective copyrights, licenses and notices. This
project's license neither replaces those licenses nor restricts rights they
independently grant. Model weights and dependency packages are not bundled in
the tutorial. Consult their licenses when downloading, using or redistributing
them. The original project kit includes the same LICENSE as this repository.

## GitHub Pages publishing

Target repository: https://github.com/rajarshi-personal/language-model-development-tutorial

Intended tutorial URL (available after a successful deployment):
https://rajarshi-personal.github.io/language-model-development-tutorial/

In the repository's **Settings → Pages → Build and deployment**, select
**GitHub Actions** as the source. The included `.github/workflows/pages.yml`
publishes from the repository's default branch when the HTML, license or
workflow changes; it can also be run manually from that branch.

The deployment artifact contains only `index.html`, `LICENSE` and `.nojekyll`.
Local verification files and the repository README are not website artifacts.
GitHub Pages is the sole hosting target configured by this project. Deployment
still requires repository access, Pages eligibility and a successful Actions run.

A repository's normal file viewer displays HTML source; GitHub Pages serves the
website. A public static website cannot prevent visitors from downloading its
HTML. A canonical URL identifies the intended hosted version, not an access
restriction. The single HTML remains self-contained.

## Included learning activities

- A build studio that maps facts, response style, or both to a concrete build
  strategy, artifacts and evaluation criteria
- A six-policy Acorn handbook inspector with JSON and JSONL previews, explicit
  training/validation/test topic labels, and source-to-example explanations
- A controllable training versus inference walkthrough using the same POST
  question, with visible target availability and weight-update counters
- An animated LoRA lifecycle (attach, update, save, use) and a calculated matrix
  experiment showing how adapter values affect a frozen base's output
- Expandable lesson explanations and practical exercises in all eight lessons
- An animated question-to-answer pipeline
- A RAG / fine-tuning / pretraining decision explorer
- Next-token probability and temperature experiments
- An editable training-record preview
- Theory before every implementation block, using the same Acorn policy example
- A narrated, controllable handbook-to-index / examples-to-weights animation
- A computed vector-similarity lab that demonstrates lexical synonym failures
- A complete retrieval-to-answer animation, including policy updates and abstention
- A local retrieval playground with visible evidence
- LoRA parameter and quantization-size calculators
- An overfitting explorer and failure diagnosis exercises
- Quizzes, saved lesson progress and a release checklist

All CSS, JavaScript, visuals and project-file contents are embedded. The page
has no external fonts, scripts, images or telemetry. Documentation links open
external websites only when followed. Theme and progress use browser-local
storage when available.

## Validation performed

- October 7 workshop update: verified all new selectors, six policy records,
  JSON/JSONL structure, held-out topic labels, loop navigation, playback/pause,
  mode-switch cancellation, adapter lifecycle and numeric slider results.
- Rechecked existing preparation, retrieval, vectors, quizzes and animations;
  all scripts parsed and Chrome reported zero JavaScript runtime exceptions.
- Checked the four new workshops at 1440, 390 and 320 px, including dark theme
  and reduced motion, with network access disabled and no page overflow.
- Compared all 22 embedded project files with the previous Git revision;
  their contents, including the license, are unchanged by this update.
- Opened the page in headless Chrome with network access disabled.
- Checked the main controls, deployment switch, quizzes and progress tracking.
- Checked both preparation paths, animation playback/pause/reset, vector scores,
  updated-policy and unknown-question walkthroughs, and reduced-motion support.
- Checked desktop (1440 px) and mobile (390 px) layouts and both themes;
  no horizontal page overflow or JavaScript runtime errors were observed.
- Verified the generated ZIP's CRCs, all 22 entries, the embedded license and
  its exact agreement with the repository LICENSE; original code files remain
  unchanged by the licensing update.
- Parsed all Python scripts, ran the sample-data generator and verified record
  counts, JSONL formatting, answer line breaks and held-out topic separation.
- Compiled the Java example with JDK 17.

GPU training, model inference, GGUF conversion and hosted deployment were not
executed in this environment. The tutorial labels simulated outputs and does
not claim model-quality improvements. Training targets Python 3.11 and a pinned
teaching stack; local Python syntax/data checks used Python 3.10.11.

Copyright © 2026 Rajarshi Ray — rajarshir@gmail.com
