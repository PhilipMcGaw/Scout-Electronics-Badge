# Agent Instructions

## Project purpose

`Scout-Electronics-Badge` is the working project for the Scouts Electronics Activity Badge booklet and related learning resources, including planned blog updates.

The intended readers are Scouts and Explorers aged 10 to 16, working with an adult Leader. Keep explanations practical, age-appropriate, and technically accurate. When adapting supplied transcripts or notes, distinguish source material from editorial explanations and Philip’s own experience. Do not invent personal experiences, equipment settings, tests, or results. Check product-specific safety, storage, and operating instructions where they matter.

## UK context and source relevance

This is a UK-centric project. Use UK Scout requirements and UK safety, legal, regulatory, and standards guidance where applicable. Electrical conventions, terminology, suppliers, and requirements can differ between territories. A US or other overseas source may be accurate in its own context but incorrect or unsuitable here. Treat it as background, verify relevant claims against current UK primary or authoritative sources before adapting them, and identify any information that applies only outside the UK.

## Language and house style

- Write new project content in British English. Use `organisation`, `organise`, `licence` as a noun, `license` as a verb, `colour`, and `behaviour`. Use `program` for software and `programme` for organised activities.
- Write clearly, concisely, and directly. Prefer familiar words and active voice. Keep technical terms consistent and explain unfamiliar terms where the intended reader may need help.
- Keep quotations, source material, product names, technical identifiers, and code faithful to their originals. Distinguish editorial text from quoted or historical source material.
- Use Unicode where appropriate. Write dates as `YYYY-MM-DD` and use SI units with a non-breaking space between the number and unit, for example `5 V` and `25 °C`. When an external source gives imperial measurements, retain them and add an appropriately rounded SI equivalent where useful.
- Use a conversational, matter-of-fact voice for articles. Retain supported first-person experiences and preferences, but do not invent them. State uncertainty plainly and avoid promotional language or unsupported claims.

## Images and licensing

- Use non-AI images or illustrations under a licence that permits the intended use. Check attribution, modification, and redistribution conditions. Do not generate an AI image when a suitable Creative Commons-licensed image is available.
- For the Scouts booklet, add a new image only when an explicit user request or TODO asks for one. Record its creator, source, licence, and required attribution beside the image or in a sources section. Prefer simple, age-appropriate diagrams that explain a component, measurement, or circuit.

## Purchasing links

When recommending websites to buy electronic parts or kits, consider [Pimoroni](https://shop.pimoroni.com/), [The Pi Hut](https://thepihut.com/), and [Kitronik](https://kitronik.co.uk/) when they stock a suitable item. Kitronik is a suggested UK source for educational electronics kits and project parts. Philip also recommends [SparkFun](https://www.sparkfun.com/), a US-based supplier; label it as an overseas option, not a UK supplier, and remind UK buyers to check delivery and any additional charges. Check that any specific part matches the project requirements before linking to it; keep manufacturer datasheets and other technical references separate from sales links.

## TODO workflow

At the start of project work, review `TODO.md` and `memories.md`. Address relevant TODOs where practical. Keep task descriptions concise, update them when scope or dependencies change, and mark work complete only after verification. `TODO.md` is the project’s action index.

`memories.md` is the default place to preserve durable project context so it carries across conversations. As part of substantive work, add or update a concise, dated entry when the user supplies a lasting preference, project decision, source assessment, or outcome that will help future work. Do this by default without asking. Keep the notebook useful rather than transcribing conversations: distinguish user-reported preferences from checked repository facts, source claims, inference, and unresolved points. Do not record secrets or personal details that are not needed for the project. Keep actionable work in `TODO.md`; link to it from a memory entry when useful, and do not duplicate the task list. Correct or remove stale memories when later information supersedes them. If work creates no durable context worth retaining, no memory entry is needed.

## Workspace restrictions

Stay within the current `Scout-Electronics-Badge` repository. Do not read, write, create, modify, move, or delete files outside it, and keep temporary or generated output inside the repository.

When the user explicitly supplies a pasted-text attachment as source material, you may read only the exact attachment path given in that message. Do not enumerate or access other files in its directory, and do not copy or move the attachment. Keep analysis and project changes inside the repository. Do not include credentials or secrets from a supplied source in project files.

## Git workflow

- On Windows, use GitHub Desktop for repository status, reviewing changes, staging selected files, committing, fetching, integrating remote changes, and pushing. If the application is unavailable or cannot perform a required operation, use the documented bundled Git executable and explain that fallback in the task report.
- On this Windows installation, use `C:\Users\philip.mcgaw\AppData\Local\GitHubDesktop\app-3.6.10\resources\app\git\cmd\git.exe` when command-line Git is needed. Verify the executable with `git --version`; the path may change after a GitHub Desktop upgrade.
- Before pushing, fetch the configured remote and integrate its latest `main` branch into the task branch. Resolve divergence or conflicts while preserving unrelated work, then review the final diff.
- Commit and push task-related changes to the configured remote’s `main` branch when the requested work is complete. Stage only files belonging to the task, review staged files before committing, and use a concise, focused commit subject.
- A user request to prepare or update repository content authorises agents to complete this commit-and-push workflow for the resulting task changes; do not ask for a separate confirmation to push. This instruction does not override filesystem or network restrictions imposed by the execution environment.
- Do not include temporary files, local configuration, secrets, or unrelated user changes unless explicitly requested. At completion, report the commit and remote branch after a successful push; if pushing is blocked, report the specific blocker.

## Text encoding and line endings

- Read and write repository text files as UTF-8 explicitly. In PowerShell, use `[System.IO.File]::ReadAllText(..., [System.Text.Encoding]::UTF8)` and `[System.IO.File]::WriteAllText(..., [System.Text.UTF8Encoding]::new($false))` for files containing non-ASCII text.
- Repository text files use LF (`\n`) line endings. Avoid mixed line endings and line-ending-only changes. Preserve binary file contents and line endings.
- After editing non-ASCII text, read it back as UTF-8 and check the affected content for mojibake, replacement characters, or unintended control characters.
