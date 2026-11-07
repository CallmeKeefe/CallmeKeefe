# Steven Keefe

**AI systems · software engineering · open source**

I build software and experiment with intelligent systems, with a focus on **AI evaluation, developer tools, and practical applications**. I’m interested in the difference between a system that looks impressive in a demo and one that behaves reliably when someone actually uses it.

[Portfolio](https://keefe.is-a.dev) · [GitHub repositories](https://github.com/CallmeKeefe?tab=repositories) · [Hugging Face](https://huggingface.co/KeefeBuild)

<p align="center">
  <img src="assets/profile-header.svg" alt="A dark geometric composition combining a terminal prompt, a Xiangqi board, and a Western chessboard" width="100%" />
</p>

---

## Selected work

A small selection of projects across AI evaluation, developer tooling, and applications. The links go directly to a demo, source repository, or published dataset so you can inspect the work.

### [LLM Hallucination Checker Edge](https://github.com/CallmeKeefe/llm-hallucination-checker-edge)

**Diagnostics for the structure of generative-AI traces.**

An OpenTelemetry-oriented tool that parses GenAI spans and flags structural signals such as empty completions, missing citation markers, and missing model metadata. It uses deterministic heuristics rather than an external LLM judge.

- [Try the web demo](https://llm-hallucination-checker.pages.dev/)
- [Read the source and methodology](https://github.com/CallmeKeefe/llm-hallucination-checker-edge)

*Important boundary: this is a trace-triage tool, not a factuality detector. Its score is not a probability that an answer is true or false.*

### [VoxShift](https://github.com/CallmeKeefe/Vox-Shift)

**An audio workspace for transcription, translation, and transcript workflows.**

The project combines a Next.js application with a separate Python-based audio-provider service. The repository documents the web interface, API, persistence layer, and provider components.

- [Open the application](https://vox-shift.vercel.app/)
- [Inspect the repository](https://github.com/CallmeKeefe/Vox-Shift)

*The project is under active development; available features depend on deployment configuration and external providers.*

### [Keefe Calculator](https://github.com/CallmeKeefe/Keefe-Calculator)

**A browser-based workspace for working with mathematics.**

It brings together a scientific calculator, function graphing, unit conversion, constants, and calculation history, with optional cloud and AI integrations.

- [Open the calculator](https://keefe-calculator.vercel.app/)
- [Inspect the source](https://github.com/CallmeKeefe/Keefe-Calculator)

*The application is not a standalone computer-algebra system. Optional integrations depend on their service configuration.*

### [Data-Provecta](https://huggingface.co/datasets/KeefeBuild/Data-Provecta)

**Dataset research for evaluating language-model behavior.**

Explores how models handle state tracking, conflicting evidence, tool grounding, and consistency across structured scenarios.

- [Explore the dataset on Hugging Face](https://huggingface.co/datasets/KeefeBuild/Data-Provecta)

---

## More experiments

<details>
<summary><strong>Models, systems, and strategy software</strong></summary>

### [Keefe-Discere](https://huggingface.co/KeefeBuild/Keefe-Discere)

A Qwen2.5-based model fine-tuning project. The Hugging Face page contains the published model artifacts and project details.

### [KeefeOS](https://github.com/CallmeKeefe/Keefe-OS)

An experimental x86-64 operating-system prototype exploring a UEFI boot path and kernel foundations. The repository documents QEMU/OVMF test evidence and the current limitations. It is not a general-purpose OS installer and does not claim physical-hardware support.

### [Xiangqi Game](https://github.com/CallmeKeefe/xiangqi-game)

A self-contained browser-based Chinese chess game. It supports local two-player play and a built-in AI opponent with selectable difficulty. The repository explains how to run it locally; it is not an online multiplayer service.

</details>

## Current interests

- **AI evaluation:** measuring consistency, state tracking, and whether model outputs are supported by the available evidence.
- **Developer tooling:** making complex systems easier to inspect, test, and debug.
- **Systems engineering:** learning how software behaves across application, infrastructure, and low-level boundaries.

## Tools I use

<details>
<summary><strong>Languages, frameworks, and infrastructure</strong></summary>

| Area | Tools used across projects |
|:--|:--|
| Languages | Python, Rust, C++, TypeScript, JavaScript |
| AI and data | PyTorch, Hugging Face, Transformers, Unsloth |
| Web | React, Next.js, Vite, Node.js, Tailwind CSS |
| Infrastructure | Vercel, Firebase, Supabase, GitHub Actions, Docker |

This is a map of tools used in my projects, not a claim of equal expertise in every item.

</details>

## Outside the terminal

Xiangqi, chess, and Go are long-running interests. I also write fiction and spend time with music, including piano and the erhu.

---

<p align="center">
  <strong>Build it. Test it. Explain its limits.</strong><br/>
  <a href="https://keefe.is-a.dev">Portfolio</a> ·
  <a href="https://github.com/CallmeKeefe">GitHub</a> ·
  <a href="https://huggingface.co/KeefeBuild">Hugging Face</a>
</p>
