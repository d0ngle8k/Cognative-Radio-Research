# Cognative-Radio-Research

## Overview

This repository is a personal collection of research material about Cognitive Radio, Software-Defined Radio (SDR), and related wireless communications topics. It collects PDFs and presentation slides (academic papers, book chapters, and lecture materials) that are useful for study and research.

The repository currently contains several large binary files (PDFs and a PowerPoint) and a short project README and LICENSE.

## Contents

- `README.md` — this file.
- `LICENSE` — the repository license (GNU GPL v3).
- Multiple research PDFs and one PPTX, including (examples):
  - `Cognative Radio Research.pdf`
  - `Cognitive Radio Communications and Networks - A. Wyglinski.pdf`
  - `Cognitive Radio Network Mahmoud.pdf`
  - `Cognitive Radio, Software Defined Radio, Arslan.pdf`
  - `Cognitive_radio_network_architecture_part_I_general_structure.pdf`
  - `Fette B.A.(ed) Cognitive Radio Technology.pdf`
  - `Thomas W. Rondeau, Charles W. Bostian-Artificial Intelligence in Wireless Communications (Mobile Communications) (2009).pdf`
  - `cognative-radio-powerpoint.pptx`
  - `cognitive-radio.pdf`

If you'd like a full machine-readable index (JSON/CSV) of the files, I can add one.

## Purpose

This repo is intended as a read-only archive and personal reference for study and research into cognitive radio systems, network architectures, and related topics. It is not an application or code library.

## License

Files in this repository are provided under the terms of the GNU General Public License v3 (GPL-3.0). See `LICENSE` for the full text.

Note: Some documents may be third-party publications; ensure you respect the original authors' rights and the terms under which those documents were obtained before redistributing.

## Large files and recommended workflow

Several PDFs and the PPTX are large binary files. For a healthier Git history and to avoid bloating the repository, consider using Git LFS for future large files.

If you or contributors plan to add large binaries, these quick steps will help on Windows PowerShell:

1. Install Git LFS (if not present):

	- Download & install from https://git-lfs.github.com/ or run `git lfs install` after installing.

2. Track file types (example):

	```powershell
	git lfs track "*.pdf"
	git lfs track "*.pptx"
	git add .gitattributes
	```

3. Re-add large files (if you want them managed by LFS) and commit:

	```powershell
	git rm --cached *.pdf *.pptx
	git add -A
	git commit -m "chore: migrate large files to git-lfs"
	git push
	```

If you need, I can help migrate existing large files to Git LFS (this rewrites recent history and requires force-push or an alternate strategy; I will explain options before doing it).

## Structure and contributions

This repository is currently a flat collection of documents. Suggested structure (optional) if you want to expand it:

- `/papers/` — published papers and book chapters (PDF)
- `/slides/` — lecture slides and presentations (PPTX/PDF)
- `/notes/` — plain-text notes, scripts, or data extracts

If you'd like me to reorganize the repo into folders and move files, I can do that and create a migration commit.

Contributions: please open an Issue or PR. If adding files, prefer hosted links or small text-based contributions; for large binaries, use Git LFS or link to external storage.

## How to cite or reference

This repository is an archival collection. If you use materials from here, cite the original authors/publications directly. If you need a citation for this collection itself, use the commit hash and GitHub URL:

`https://github.com/d0ngle8k/Cognative-Radio-Research`

## Contact / Maintainer

Repository owner: d0ngle8k (on GitHub). Open an issue or contact via GitHub profile for questions or requests.

## Next steps I can help with

- Add a `.gitattributes` and enable Git LFS for PDFs/PPTX.
- Move large files into `/papers` and `/slides` folders and update README accordingly.
- Create an index file (JSON/CSV) listing file metadata (filename, size, commit, added date).

If you want any of these, tell me which and I'll implement it.
