SICE FES 2026 Tutorial
CafeOBJ example specifications and Proof Scores

Directories
-----------
ABCf, Fischer, and Vehicle each contain:

  main.cafe
    Complete specification and verification-property definitions.

  test.cafe
    Representative executable examples.

  invN.cafe
    Complete Proof Score for invariant invN.

Fischer and Vehicle also contain:

  lemmas.cafe
    Previously proved low-level helper lemmata required by the invariant
    Proof Scores.  Their proof scripts are under auxiliary/.

Vehicle additionally contains:

  safety.cafe
    Structural-induction proof of the generalized safety property.
    Its nontrivial case is reduced to invariant inv1.

  inv1.cafe
    Reachable-state Proof Score for the adjacent-pair invariant used by
    safety.cafe.

  inv2.cafe ... inv6.cafe
    Reachable-state invariant lemmata supporting the inv1 Proof Score.

Vehicle/auxiliary additionally contains:

  lemma1.cafe
    Structural-induction proof of the auxiliary PSet/c-tick lemma discussed
    in the slides.

Running an example
------------------
Start CafeOBJ in a case-study directory.  Each user-facing file loads its
own prerequisites, so use a fresh session for any file, for example:

  cd ABCf
  cafeobj
  CafeOBJ> in test.cafe

or:

  CafeOBJ> in inv1.cafe

For auxiliary proofs, start CafeOBJ in the auxiliary directory and load the
chosen file there.  For example:

  cd Fischer/auxiliary
  cafeobj
  CafeOBJ> in pset-lemmas.cafe

The auxiliary files use portable relative imports such as in ../main.cafe.
