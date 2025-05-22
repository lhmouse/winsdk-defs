This repository contains [a script](update.ast) to generate module definition
(DEF) files from import libraries of Microsoft Windows SDK.

The script is written in **Asteria**. You may obtain its source code from
https://github.com/lhmouse/asteria and compile it in MSYS2 or Cygwin.

The script uses **llvm-objdump** to parse import libraries, then uses regular
expressions to extract symbols from its output. It's slow, but fortunately we
only have to do it once for each Windows SDK release.
