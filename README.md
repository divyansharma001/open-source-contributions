# Open Source Contributions
**Divyansh Sharma** — Software Engineer

Curated log of my upstream contributions: merged PRs, active reviews, and meaningful fixes.

## Merged Contributions
Reviewed, approved, and merged into main.

### [Mogan STEM Suite](https://github.com/MoganLab/mogan)  
Professional scientific writing platform (based on GNU TeXmacs) for math, physics, stats, and CS — structured WYSIWYG editing with fast PDF/Beamer export.

- **Feb 26, 2026** [#2865](https://github.com/MoganLab/mogan/pull/2865) — Fix Latin Modern Math "h" input failure  
  Mapped problematic U+1D455 to U+210E (PLANCK CONSTANT) with substitutions; added tests and root-cause doc in `devel/206_19.md`. Closes #2742.

- **Feb 26, 2026** [#2856](https://github.com/MoganLab/mogan/pull/2856) — Use platform-native modifier names in shortcut hints  
  Replaced generic "Meta" with "Super" (Linux), "Win" (Windows), "Command" (macOS); cleaned translations and added keyboard docs. Closes #2822.

- **Feb 25, 2026** [#2847](https://github.com/MoganLab/mogan/pull/2847) — Fix unclickable hyperlinks in Beamer PDF export  
  Deferred typesetter cleanup to preserve link registrations; inlined logic + test doc. Closes #2843.

- **Feb 25, 2026** [#2845](https://github.com/MoganLab/mogan/pull/2845) — Apply "Prefix by section number" to Question/Answer environments  
  Refactored counters and macros for consistent prefixing (e.g., "Question 1.1"); aligns with theorem/exercise handling. Closes #2806.

### [DMD Compiler](https://github.com/dlang/dmd)  
Reference compiler for the D programming language — handles parsing, semantics, and code generation.

- **Feb 25, 2026** [#22622](https://github.com/dlang/dmd/pull/22622) — Fix #22567: alias this + nested AAs trigger SIGILL crash  
  Added post-rewrite lowering to treat modifiable AA indexes as rvalues; included test case. Co-authored with AI assistance.

- **Mar 2, 2026** [#22615](https://github.com/dlang/dmd/pull/22615) — Fix #22614: tmpnam() permission issues on Windows (non-admin)  
  Switched to `GetTempPathA` + `GetTempFileNameA` for safe temp files in ImportC preprocessing; added error handling. Enables non-admin druntime/phobos builds.

## In Review
Submitted and under discussion — focusing on UI reliability, command interrupts, and platform consistency.

### Mogan STEM Suite (MoganLab/mogan)
- [#2907](https://github.com/MoganLab/mogan/pull/2907) — Fix stuck PDF export wait indicator  
- [#2901](https://github.com/MoganLab/mogan/pull/2901) — Enable Cmd+V paste in macOS save dialog  
- [#2876](https://github.com/MoganLab/mogan/pull/2876) — Resolve duplicate labels in table variant dropdown  
- [#2866](https://github.com/MoganLab/mogan/pull/2866) — Implement Ctrl+G interrupt for long-running operations  
- [#2860](https://github.com/MoganLab/mogan/pull/2860) — Extend replace-all to full document (not just after cursor)  
- [#2858](https://github.com/MoganLab/mogan/pull/2858) — Disable mouse resize on matrix/det environments  

### DMD Compiler (dlang/dmd)
- [#22638](https://github.com/dlang/dmd/pull/22638) — Add @nogc to core.sys.windows.objbase functions (Fix #22573)  

## Stats
| Metric                  | Count |
|-------------------------|-------|
| PRs merged              | 6     |
| Projects contributed to | 2     |
| PRs in review           | 6     |
| Bug reports resolved    | 0     |

**Last updated:** March 2026

Manually maintained, updated whenever PRs merge or progress.
