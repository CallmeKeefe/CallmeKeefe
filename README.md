<!--
  Profile README — deep-jade terminal design with evidence-based project descriptions.
  Keep claims aligned with linked repositories and published artifacts.
-->

<p align="center">
  <img src="assets/profile-header.svg" alt="Terminal-inspired profile header with Xiangqi and chess starting positions" width="100%" />
</p>

<h1 align="center">Steven Keefe</h1>
<p align="center"><strong>AI research · software engineering · systems experiments</strong></p>
<p align="center">
  <a href="https://keefe.is-a.dev">Portfolio</a> ·
  <a href="https://github.com/CallmeKeefe?tab=repositories">GitHub projects</a> ·
  <a href="https://huggingface.co/KeefeBuild">Hugging Face</a>
</p>
<p align="center"><sub>Curiosity starts the build. Evidence decides whether it works.</sub></p>

---

## $ whoami

I'm an independent developer exploring how intelligent software is designed, evaluated, and engineered—from language-model behavior to the systems underneath an application.

I learn by building things that can be inspected: web products, AI evaluation tools, model experiments, and low-level systems prototypes. I enjoy the full loop: define a problem, make a working version, test edge cases, investigate failures, document limitations, and improve the design.

**The questions that keep me building:**

- Can an AI system stay consistent when facts change or evidence conflicts?
- How can model behavior become easier to inspect, test, and evaluate?
- Can useful developer tools make complex tasks feel simpler?
- What happens between firmware, a bootloader, and a kernel?
- How can interfaces be expressive and genuinely usable?

<p align="center">
  <img src="assets/terminal-stage.svg" alt="Isometric three-dimensional terminal console showing a build, test, inspect workflow" width="100%" />
</p>

### A small terminal snapshot

~~~text
             .--------------------------------------.
            /  KEEFE / WORKBENCH                   /|
           /--------------------------------------/ |
           |  $ whoami                            | |
           |  independent developer               | |
           |                                      | |
           |  $ focus                             | |
           |  AI evaluation  /  software          | |
           |  systems        /  open source        | |
           |                                      | /
           '--------------------------------------'

  build  ->  test  ->  inspect  ->  document  ->  improve
~~~

---

## $ tree ./work --depth=2

A map of the problems and products I work on:

<p align="center">
  <img src="assets/project-map.svg" alt="Six project areas: trace diagnostics, audio workflows, math tools, model evaluation, language model experiments, and operating-system foundations" width="100%" />
</p>

### 01 · LLM Hallucination Checker Edge

**Inspect structural warning signs in LLM traces.**

An OpenTelemetry-oriented diagnostic utility that parses GenAI trace spans and flags signals such as empty completions, missing citation markers, and missing model metadata. It has a Python core, a dependency-free edge Worker, a browser widget, and a command-line interface.

- Deterministic heuristics; no external LLM judge is required.
- Supports local trace scoring in the browser and trace-file evaluation from the CLI.
- Includes tests across the Python and Worker implementations.

[Repository](https://github.com/CallmeKeefe/llm-hallucination-checker-edge) · [Live demo](https://llm-hallucination-checker.pages.dev/)

<sub>Boundary: this is a structural triage tool, not a factuality detector. Its score is not a probability that an answer is hallucinated.</sub>

### 02 · VoxShift

**A workspace for speech and transcript workflows.**

A deployed web application focused on transcription, translation, and working with generated transcripts. The product separates its web experience from audio-provider functionality.

[Open VoxShift](https://vox-shift.vercel.app/)

<sub>The demo is public; its source repository is currently private. Provider availability and deployed features may change.</sub>

### 03 · Keefe Calculator

**A browser-based environment for mathematical exploration.**

A multi-tool math workspace bringing together scientific calculation, function graphing, unit conversion, constants, and calculation history, with optional cloud and AI integrations.

[Open Keefe Calculator](https://keefe-calculator.vercel.app/)

<sub>The demo is public; its source repository is currently private. It is a practical math workspace, not a full computer-algebra system.</sub>

### 04 · Data-Provecta

**A dataset for evaluating long-horizon grounded reasoning.**

Data-Provecta studies whether models can maintain a reliable view of the world as new evidence arrives, facts change, tools disagree, and misleading information appears.

Its scenario design separates authoritative state from observable evidence. The dataset includes versioned examples, train/validation/test splits, difficulty metadata, and adversarial variants such as stale evidence, red herrings, authority conflicts, and conflicting tool outputs.

- **80 published rows** on the current Hugging Face dataset page.
- A canonical schema and state-machine-oriented ground truth.
- Evaluation dimensions include temporal consistency, tool grounding, conflict resolution, and uncertainty calibration.
- Designed for research and evaluation—not as a guarantee of model safety or correctness.

[Dataset](https://huggingface.co/datasets/KeefeBuild/Data-Provecta)

### 05 · Keefe-Discere

**An open model-development and fine-tuning experiment.**

A Qwen2.5-7B-based model project exploring instruction tuning and code/tool-use behavior. The Hugging Face repository publishes model artifacts in formats including GGUF and Safetensors, with usage paths for Transformers and llama.cpp.

[Model and files](https://huggingface.co/KeefeBuild/Keefe-Discere)

<sub>Published artifacts and model revisions are experimental; results depend on the exact revision, runtime, quantization, and hardware.</sub>

### 06 · KeefeOS

**Learning systems engineering from the boot path upward.**

An experimental x86-64 operating-system prototype built around a UEFI loader, a Rust kernel, a boot protocol, and QEMU/OVMF testing.

The repository documents successful early-boot checks across 256 MiB, 512 MiB, and 1 GiB QEMU memory profiles. It also documents what is not ready: physical installation, broad hardware support, a complete driver stack, and production security.

[Repository](https://github.com/CallmeKeefe/Keefe-OS) · [Build and boot guide](https://github.com/CallmeKeefe/Keefe-OS/blob/main/docs/BUILD_AND_BOOT_GUIDE.md) · [CI history](https://github.com/CallmeKeefe/Keefe-OS/actions)

---

## $ ls ./side-projects

### Xiangqi — Chinese Chess

A self-contained browser game with local two-player play and an AI opponent with selectable difficulty. It includes move history, undo, new-game controls, sound, and an in-page analysis panel.

[Source code and run instructions](https://github.com/CallmeKeefe/xiangqi-game)

<sub>Local browser game; no online multiplayer. Difficulty labels describe application settings, not tournament-engine strength.</sub>

---

## $ cat interests.txt

| Area | What I like exploring |
|:--|:--|
| **AI evaluation** | State tracking, consistency, grounded tool use, uncertainty, and adversarial testing |
| **Model development** | Fine-tuning workflows, inference formats, quantization, and reproducible experiments |
| **Developer tools** | Diagnostics, automation, useful interfaces, and testable workflows |
| **Systems engineering** | Rust, boot protocols, memory management, kernel boundaries, and virtual-machine testing |
| **Product engineering** | Responsive web apps, interaction design, performance, and deployment |
| **Strategy games** | Xiangqi, chess, Go, and the design of game-playing systems |

## $ stack --from-projects

<details>
<summary><strong>Languages, frameworks, and tools used across my projects</strong></summary>

| Layer | Technologies |
|:--|:--|
| Languages | Python · Rust · C++ · TypeScript · JavaScript |
| AI and data | PyTorch · Hugging Face · Transformers · Unsloth · Pydantic |
| Web | React · Next.js · Vite · Node.js · Tailwind CSS |
| Systems | UEFI · x86-64 · QEMU · OVMF |
| Infrastructure | GitHub Actions · Vercel · Cloudflare Workers · Firebase · Supabase · Docker |
| Quality | pytest · Node test runner · Clippy · RustSec · CI workflows |

<sub>This is a map of technologies used across different projects—not a claim of equal expertise in every tool.</sub>
</details>

---

## $ principles

- **Build in public where possible.** Make the work inspectable and invite useful feedback.
- **Prefer evidence over impressive wording.** A passing test proves only what that test covers.
- **Keep limitations visible.** A prototype should be described as a prototype.
- **Design for the person using it.** Clarity, accessibility, responsiveness, and performance matter.
- **Treat setbacks as information.** Find the failing assumption, test it, and iterate.

<p align="center">
  <img src="assets/terminal-divider.svg" alt="Terminal prompt divider" width="100%" />
</p>

<p align="center">
  <strong>Make it useful. Make it testable. Make it better.</strong><br />
  <a href="https://keefe.is-a.dev">Portfolio</a> ·
  <a href="https://github.com/CallmeKeefe">GitHub</a> ·
  <a href="https://huggingface.co/KeefeBuild">Hugging Face</a>
</p>
