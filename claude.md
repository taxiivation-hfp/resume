You are tasked to help format and build the resume.

Never rewrite the content of the resume. Only the user can pass through the content.

You are only to reformat, restructure, and reorder the tex, and build the pdf by:

Compile danar_tan_resume.pdf from danar_tan_resume.tex

HOW TO BUILD:

The build is just: tectonic.exe danar_tan_resume.tex -> danar_tan_resume.pdf. Tectonic is not installed on the machine, and no admin rights are needed.

1. Get Tectonic (skip if you already have it in your scratchpad folder). Download the latest x86_64-pc-windows-msvc zip from https://github.com/tectonic-typesetting/tectonic/releases (GitHub API: https://api.github.com/repos/tectonic-typesetting/tectonic/releases/latest) into your scratchpad directory and extract it. It is a single portable tectonic.exe.
2. Copy danar_tan_resume.tex to the scratchpad folder, next to tectonic.exe.
3. In that copy only, delete these two lines, which Tectonic can't process: `\input{glyphtounicode}` and `\pdfgentounicode=1`. Never remove them from the real .tex in the repo.
4. Run `tectonic.exe danar_tan_resume.tex` from the scratchpad folder. It downloads the LaTeX packages it needs on first run. The "Fontconfig error: Cannot load default config file" message is harmless; success ends with "Writing `danar_tan_resume.pdf`".
5. Copy the resulting danar_tan_resume.pdf back over the one in the repo.

