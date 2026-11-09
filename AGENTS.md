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

## Canonical DokuWiki page layout

The source-controlled DokuWiki pages are the canonical editable project documents. Use these repository paths and namespace IDs:

- Root landing page: `pages/sites/scouts-electronics-badge/start.txt` (`sites:scouts-electronics-badge:start`)
- Badge booklet: `pages/sites/scouts-electronics-badge/booklet.txt` (`sites:scouts-electronics-badge:booklet`)
- Leaders’ Guide: `pages/sites/scouts-electronics-badge/leaders-guide.txt` (`sites:scouts-electronics-badge:leaders-guide`)
- Blog index and drafts: `pages/sites/scouts-electronics-badge/blog/start.txt` and `pages/sites/scouts-electronics-badge/blog/<page-id>.txt` (`sites:scouts-electronics-badge:blog:<page-id>`)
- Source reviews and indexes: `pages/sites/scouts-electronics-badge/sources/start.txt` and `pages/sites/scouts-electronics-badge/sources/<page-id>.txt` (`sites:scouts-electronics-badge:sources:<page-id>`)
- Booklet media: `media/sites/scouts-electronics-badge/`, under namespace `sites:scouts-electronics-badge`

Keep page and media directories parallel to their namespace paths. Use UTF-8 `.txt` page files, lowercase kebab-case page IDs, and a `start.txt` landing page in every namespace directory. Use fully qualified DokuWiki namespace IDs for internal links, for example `[[sites:scouts-electronics-badge:booklet|Badge booklet]]`; use fully qualified media IDs for media references, for example `{{sites:scouts-electronics-badge:diagram.png|Circuit diagram}}`. Use DokuWiki core syntax for links, media, headings, lists, tables, and code. Do not rely on Markdown rendering or plugin syntax, including metadata macros, unless the target DokuWiki installation is confirmed to have the required plugin enabled. No page-metadata convention is established: do not add front matter or invent plugin metadata. Use a leading core-syntax heading for the visible page title and keep source, attribution, and licence details in the page body.

Repository administration files (`AGENTS.md`, `TODO.md`, `memories.md`, and Git metadata), KiCad design/source files, and original source documents are not DokuWiki pages by default. Do not copy whole source or design directories into media. Select individual reference attachments only when they are useful, readable, and permitted for the intended use; keep their source and licence information traceable.

The repository’s `.txt` pages remain canonical when preparing a target DokuWiki instance. Verify page content, namespace IDs, media and internal links in that instance before editing the live pages or changing the editing workflow to use the instance.

## TODO workflow

At the start of project work, review `TODO.md` and `memories.md`. Address relevant TODOs where practical. Keep task descriptions concise, update them when scope or dependencies change, and mark work complete only after verification. `TODO.md` is the project’s action index.

`memories.md` is the default place to preserve durable project context so it carries across conversations. As part of substantive work, add or update a concise, dated entry when the user supplies a lasting preference, project decision, source assessment, or outcome that will help future work. Do this by default without asking. Keep the notebook useful rather than transcribing conversations: distinguish user-reported preferences from checked repository facts, source claims, inference, and unresolved points. Do not record secrets or personal details that are not needed for the project. Keep actionable work in `TODO.md`; link to it from a memory entry when useful, and do not duplicate the task list. Correct or remove stale memories when later information supersedes them. If work creates no durable context worth retaining, no memory entry is needed.

## Workspace restrictions

Stay within the current `Scout-Electronics-Badge` repository. Do not read, write, create, modify, move, or delete files outside it, and keep temporary or generated output inside the repository.

When the user explicitly supplies a pasted-text attachment as source material, you may read only the exact attachment path given in that message. Do not enumerate or access other files in its directory, and do not copy or move the attachment. Keep analysis and project changes inside the repository. Do not include credentials or secrets from a supplied source in project files.

## Git workflow

Standing authorisation: For user-requested changes in this repository, agents are authorised to stage the required files, commit focused validated changes, and push them to the configured remote and current working branch without asking the user again. This authorisation does not override sandbox or authentication controls; if a Git operation is blocked, report the specific blocker.

Before editing, inspect the complete working-tree status and relevant diffs. Preserve unrelated changes, and stage only files required for the task.

Review the staged diff before committing. Use focused changes with clear, imperative commit subjects of 72 characters or fewer.

On Windows, use GitHub Desktop as the default interface for repository status, reviewing diffs, staging selected files, committing, fetching, integrating remote changes, and pushing. Do not assume Git is unavailable because `git` is not on PowerShell's `PATH`.

Use command-line Git only when GitHub Desktop cannot perform a required operation, is unavailable, or repeatable automation is materially more appropriate. On Windows, use a repository helper such as `tools/github-desktop-git.cmd` when present. If no helper is available, use the documented GitHub Desktop bundled Git executable for the current host; recheck its path and version after GitHub Desktop upgrades. On macOS, use command-line Git from this repository's working directory and the machine's configured authentication.

On Windows host `GBR-3N87GR3`, the documented GitHub Desktop 3.6.7 executable is `C:\Users\philip.mcgaw\AppData\Local\GitHubDesktop\app-3.6.7\resources\app\git\cmd\git.exe` (`git version 2.53.0.windows.4`, checked 2026-10-09). Use it when the Desktop interface cannot perform a required operation; recheck after upgrades.

Before pushing, fetch the configured remote and integrate its latest branch into the task branch. Resolve divergence while preserving unrelated work, then review the final diff and push. Do not expose credentials or tokens.

Use focused changes with clear commit messages. After a requested change has been validated, create the focused commit and push it to the configured remote and current working branch as part of the normal workflow, unless the user explicitly asks to stop before committing or pushing, or a concrete blocker prevents it. Before staging, inspect the complete status and diff so that unrelated work is not included. Do not rewrite history, force-push, reset unrelated work, or include unrelated changes. The default branch is main unless the repository states otherwise.

## Text encoding and line endings

- Read and write repository text files as UTF-8 explicitly. In PowerShell, use `[System.IO.File]::ReadAllText(..., [System.Text.Encoding]::UTF8)` and `[System.IO.File]::WriteAllText(..., [System.Text.UTF8Encoding]::new($false))` for files containing non-ASCII text.
- Repository text files use LF (`\n`) line endings. Avoid mixed line endings and line-ending-only changes. Preserve binary file contents and line endings.
- After editing non-ASCII text, read it back as UTF-8 and check the affected content for mojibake, replacement characters, or unintended control characters.
