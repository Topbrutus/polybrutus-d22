# Polybrutus 22D: Exact Euclidean Completion and a Sixteenfold Weighted-Graph Mode

**Research author:** Gabriel St-Pierre  
**Affiliation:** Independent researcher  
**Programme:** Polybrutus-X72  
**Date:** 20 November 2026  
**Version:** 0.1.0  
**Status:** Reproducible computational mathematics preprint, not independently peer reviewed by human researchers  
**Immutable predecessor:** Polybrutus 21D, DOI 10.5281/zenodo.24409527  
**Frozen scientific source:** https://github.com/Topbrutus/polybrutus-d22/tree/v0.1.0 (upon release)

## Abstract

We construct a particular exact **twenty-seven-point labelled Euclidean distance configuration** whose minimum affine embedding dimension is **twenty-two**. All **325 predecessor labelled squared pairwise distances** are conservatively preserved from the archived Polybrutus 21D geometry. One additional perpendicular radius-R point introduces **26 new squared pair distances of exactly 2R²**, yielding **351 labelled unordered pair distances** distributed among eight normalized distance classes. Exact coordinate-difference and centered squared-distance Gram ranks both equal 22, and an exact positive-semidefinite Gram factorization certifies Euclidean realizability. A separately implemented rational checker reproduces all 351 labelled squared distances and independently confirms Gram rank 22.

For a **chosen ideal complete weighted-graph scalar-oscillator model**, with equal unit masses and couplings `w_ij=R²/d_ij²`, the exact 27-by-27 graph Laplacian has eigenvalue **27/2 with multiplicity sixteen** and eigenvalue **13 with multiplicity four**. Both exact characteristic-polynomial results are independently checked by distinct symbolic and rational programs. This is a mathematical model-specific case study, **not evidence of physical twenty-two-dimensional spacetime, measured frequencies, new particles or a novel universal theorem**.

## 1. Provenance and original seven-point geometry

The Polybrutus programme originates with seven exactly defined radius-R points on a sphere embedded in three-dimensional Euclidean space. The first conservative extension introduced five centered regular-simplex vertices in a perpendicular four-dimensional subspace, retaining the original seven points. That original 7D affine metric has twelve points and sixty-six labelled pair distances (DOI **10.5281/zenodo.24407952**).

Subsequent dimension-specific archives conservatively extended the labelled geometry by one orthogonal radius-one direction per dimension: 8D (13 vertices, 78 pairs, DOI 10.5281/zenodo.24408344); 9D (14, 91, 10.5281/zenodo.24408448); 10D (15, 105, 10.5281/zenodo.24408569); 11D (16, 120, 10.5281/zenodo.24408650); 12D (17, 136, 10.5281/zenodo.24408720); 13D (18, 153, 10.5281/zenodo.24408769); 14D (19, 171, 10.5281/zenodo.24408836); 15D (20, 190, 10.5281/zenodo.24408887); 16D (21, 210, 10.5281/zenodo.24408979); 17D (22, 231, 10.5281/zenodo.24409067); 18D (23, 253, 10.5281/zenodo.24409207); 19D (24, 276, 10.5281/zenodo.24409343); 20D (25, 300, 10.5281/zenodo.24409424); 21D (26, 325, 10.5281/zenodo.24409527).

The present 22D study derives **only from the immutable scientific Git tag** `Topbrutus/polybrutus-d21@v0.1.0`, source commit **`f17e4d02f7442d18cdafbcbb0b62380c557e4ef2`**. Earlier source programs and exact certificates are copied without changing their content into the archive directory `prior/`. No old point, source tag, DOI or previous published geometry is changed.

## 2. Exact 27-point Euclidean construction

Normalize radius to `R=1` and denote the 26 frozen predecessor unit vectors by `p1,...,p26`, represented in 22 coordinate-storage slots. The original five-point regular-simplex block lies in a centered four-dimensional hyperplane, imposing one exact linear relation on its five slots.

Append a zero coordinate to each old vector:

```
q_i=(p_i,0),            i=1,...,26.
```

Add the new perpendicular unit vector in the twenty-third storage slot:

```
q27=e23=(0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,1).
```

All points have unit norm, and `q27` is orthogonal to every predecessor point. Thus all **325 exact previous labelled squared distances remain unchanged**. For each of the 26 new pairs:

```
||q27-q_i||²=||q27||²+||q_i||²-2<q27,q_i>=2.
```

Scaling all coordinates by any radius `R>0` multiplies the squared distances by `R²`; every new squared pair distance is therefore `2R²`. The total number of unordered labelled pairs is

```
C(27,2)=351=325+26.
```

With the exact normalized squared-distance class `k=4d²/R²`, the complete histogram is

| k | 4 | 7 | 8 | 9 | 10 | 12 | 13 | 16 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Labelled pairs | 6 | 2 | **320** | 3 | 10 | 6 | 2 | 2 |

These multiplicities sum to 351, and the complete squared-distance sum is

```
sum_{i<j}d_ij²/R²=2855/4.
```

At radius one the centroid in the 23 storage slots is

```
G=(0,0,1/54,0,0,0,0,0,1/27,1/27,1/27,1/27,1/27,1/27,
   1/27,1/27,1/27,1/27,1/27,1/27,1/27,1/27,1/27).
```

The final fifteen entries equal 1/27. The minimum affine dimension is 22, **not the number of storage slots 23**: the stored simplex coordinates retain one exact constraint.

## 3. Exact Euclidean distance Gram proof

Let `X` be the exact 27-by-23 stored coordinate array and `D` the exact 27-by-27 **squared Euclidean distance** matrix. Let `H=I-11ᵀ/27` be the exact centering operator. Define the centered Euclidean distance Gram matrix

```
B=-(1/2)HDH.
```

The primary exact symbolic verifier certifies, without floating-point approximation:

```
rank([q2-q1,...,q27-q1])=22;
rank(B)=22;
B=(HX)(HX)^T.
```

The last equation proves **positive semidefiniteness** of `B` through exact matrix factorization. A complete labelled squared-distance matrix uniquely determines its centered Euclidean Gram matrix. Consequently every Euclidean realization of the same **351 exact labelled squared pair distances** must have minimum affine dimension **twenty-two**. This is a statement about an abstract mathematical configuration, not about physical spacetime.

The independently implemented rational verifier does **not import the primary coordinate generator**. It reconstructs all 351 squared distances using rational structural rules for the original seven points, internal squared distances `5/2` for the five original regular-simplex vertices, and orthogonality for fifteen appended unit directions. It checks all **351/351** distances, all **325/325** frozen predecessor labelled pairs, and exact Gram rank **22**.

## 4. A sixteenfold eigenvalue in a stipulated ideal graph model

Choose a complete graph on the twenty-seven labelled points with hypothetical equal unit scalar masses and pair couplings `w_ij=R²/d_ij²`. These weights are a **model choice**, not inferred from experimental observations.

The new vertex joins all 26 predecessor vertices with normalized squared distance 2, hence every new edge weight is 1/2. If `L21` is the preceding 26-by-26 Laplacian and `L22` is the new 27-by-27 Laplacian, then

```
L22=[ L21+(1/2)I26     -(1/2)1 ]
    [ -(1/2)1ᵀ               13 ].
```

The full graph separates into the global uniform zero mode, a new intergroup mode and shifted predecessor zero-sum modes. For the monic characteristic polynomials `chi26(z)=det(zI-L21)` and `chi27(z)=det(zI-L22)`, the exact recurrence is

```
chi27(z)=z(z-27/2)chi26(z-1/2)/(z-1/2).
```

The frozen Polybrutus 21D graph polynomial is

```
chi26(z)=z(z-13)^15(z-25/2)^4*f6(z-19/2),
f6(z)=chiP7(z)/z,
```

where `chiP7` denotes the original seven-point weighted graph characteristic polynomial and `f6` its six nonzero modes. Substituting yields

```
chi27(z)=z(z-27/2)^16(z-13)^4*f6(z-10).
```

The primary program computes the **complete exact 27-by-27 characteristic polynomial** directly, then compares it to the recurrence and the closed form. Exact nonvanishing checks `f6(7/2)!=0` and `f6(3)!=0` exclude any extra coincidence at the identified eigenvalues. Hence **27/2 is exactly sixteenfold**, and **13 is exactly fourfold**.

The independent rational verifier reconstructs the full weighted graph from its own 351-pair rational distance matrix and confirms the same exact characteristic root multiplicities by derivative tests. These are **dimensionless abstract graph eigenvalues**, not physical frequencies in hertz.

## 5. Reproducibility, falsification and archival integrity

The source repository includes `src/verify_d22.py` (primary exact geometry, Gram and graph spectrum), `tests/independent_d22.py` (separately implemented rational metric and spectral checks), `results/certificate_d22.json` (complete **351-pair exact labelled metric**), frozen source and exact predecessor certificates in `prior/`, formal specification, proof, provenance, GitHub Actions workflow and Git-blob SHA-256 index.

Reproduce:

```sh
python -m pip install sympy==1.14.0
python src/verify_d22.py
python tests/independent_d22.py
```

Both programs must output PASS and the identical SHA-256 of the regenerated certificate. Four adversarial false cases are detected: one altered labelled distance, a duplicated new vertex causing affine rank loss, a nonorthogonally tilted new vector, and relabelled vertices with identical unlabelled histogram but different labelled metric.

The archived release will contain precisely three scientific artifacts: a ZIP from the **immutable tested Git tag** produced with `git archive v0.1.0`, the scientific PDF preprint, and the exact 351-pair JSON certificate. Hashes and byte lengths enable later verification of the released artifacts.

## 6. Precedence, scientific limits, authorship and disclosure

Orthogonal Euclidean completions, centered squared-distance Gram matrices and uniform weighted-graph Laplacian joins are **established mathematical techniques**. The present work documents one particular **exactly reproducible Polybrutus 22D computational case study**, not a new universal theorem or newly discovered principles of Euclidean geometry.

The exact affine rank 22 **does not establish physical extra spatial dimensions**, observed vibrations, a new elementary particle, or a new interaction. Independent human mathematical peer review has not taken place.

**Human research author and scientifically responsible investigator:** Gabriel St-Pierre, independent researcher, who originated and directs the Polybrutus programme.

**Generative AI disclosure:** OpenAI ChatGPT (Astra) substantially assisted exact symbolic mathematical verification, implementation of the main and separately programmed rational verifier, the selected theoretical graph model, scientific writing, documentation and GitHub/Zenodo archival operations. The AI system is **not a research author**.

**Licenses:** scientific preprint and prose CC BY 4.0; research source MIT.

**References:** initial Polybrutus specification https://github.com/Topbrutus/polybrutus/blob/main/SPECIFICATION.md ; frozen predecessor code https://github.com/Topbrutus/polybrutus-d21/tree/v0.1.0 ; D21 DOI https://doi.org/10.5281/zenodo.24409527 ; complete previous DOI chain in source `PROVENANCE.md`.
