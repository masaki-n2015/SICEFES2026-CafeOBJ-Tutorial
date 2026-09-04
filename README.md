# SICE FES 2026 Tutorial

Specification and Verification of Real-Time Systems Using the OTS/CafeOBJ Method: A Tutorial

Masaki Nakamura
Toyama Prefectural University

## Tutorial Paper

A preprint of the tutorial paper is available on Jxiv:

https://jxiv.jst.go.jp/index.php/jxiv/preprint/view/3874/

## Slides

The tutorial slides are available in:

[slides/sicefes_hots_beamer_presentation.pdf](slides/sicefes_hots_beamer_presentation.pdf)

## CafeOBJ files

The executable CafeOBJ specifications and Proof Scores are available under [cafeobj/](cafeobj/).

The examples are organized into five groups:

- **chap2** — introductory CafeOBJ and OTS examples used in Section 2
- **ABCt** — real-time OTS/CafeOBJ examples used in Section 3
- **ABCf** — mutual-exclusion specification and Proof Scores
- **Fischer** — Fischer's protocol case study
- **Vehicle** — autonomous vehicle control case study

The `chap2/ABCf.cafe` file is the original Section 2 tutorial source,
whereas `ABCf/` contains the participant-facing mutual-exclusion
specification and Proof Scores.

See `cafeobj/README.txt` for execution instructions.

## Requirements

CafeOBJ is required only if you want to execute the examples locally.
Installing CafeOBJ is not required to follow the tutorial, but running the
examples on your own computer can make the tutorial more interactive.

The distributed files were validated with CafeOBJ 1.6.2 (PigNose0.99).

Download and installation instructions are available from the official CafeOBJ site:

https://cafeobj.org/download/

For macOS, we recommend the official SBCL binary package from the CafeOBJ site.
As of September 2026, we have observed that the current Homebrew package may fail
to load the standard prelude on macOS, so `brew install cafeobj` is not
recommended for this tutorial.

After installation, start CafeOBJ and confirm that the startup message includes:

```text
-- CafeOBJ system Version 1.6.2(PigNose0.99) --
...
prelude file: std.bin
```

## Tutorial

SICE FES 2026

"Specification and Verification of Real-Time Systems Using the OTS/CafeOBJ Method: A Tutorial"
