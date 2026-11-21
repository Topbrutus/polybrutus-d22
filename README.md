# POLYBRUTUS 22D — Exact 27-point Euclidean metric and a sixteenfold ideal graph mode

## Official publicly verified scientific release

- **Zenodo DOI:** [10.5281/zenodo.24409636](https://doi.org/10.5281/zenodo.24409636), [public record 24409636](https://zenodo.org/records/24409636), verified through the public Zenodo API.
- **Frozen scientific source:** [`v0.1.0`](https://github.com/Topbrutus/polybrutus-d22/tree/v0.1.0), source commit `4d4e80a7156a118f8f2bebf63aca76ac5f0f06eb`.
- **Exact independent CI:** [GitHub Actions D22 run 44851196428](https://github.com/Topbrutus/polybrutus-d22/actions/runs/44851196428), conclusion `success` on the immutable scientific source; both checkers PASS.
- **Three Zenodo attachments:** immutable tagged Git source ZIP, mathematical PDF note, 351-pair exact labelled JSON distance certificate; remote checksums verified.
- **Scientific limits:** exact 22D affine Euclidean metric and chosen ideal weighted graph model. No observed physical extra dimension, measured resonance or original universal theorem claimed.


**Human research author and responsibility:** Gabriel St-Pierre, independent researcher.  
**Scientific status:** exact reproducible mathematical case study, not independently human peer reviewed.  
**AI use:** OpenAI ChatGPT (Astra) substantially assisted exact symbolic mathematics, two separately coded verification programs, selected theoretical graph model, scientific writing, documentation and controlled release. AI is not an author.

## Exact results (unit radius R=1)

- **27 labelled vertices**, **351 exact pairwise squared distances**, and minimum Euclidean affine embedding dimension **22**.
- All **325/325** labelled predecessor squared distances of frozen Polybrutus 21D are conserved. One additional perpendicular unit point creates **26 new squared pair distances**, each equal to **2**.
- Eight normalized squared-distance classes `k=4d²/R²`: `{4:6,7:2,8:320,9:3,10:10,12:6,13:2,16:2}`.
- Total squared pair distance: **2855R²/4**.
- Exact coordinate-difference affine rank **22**; exact centered Euclidean squared-distance Gram rank **22**; positive-semidefinite identity `B=(HX)(HX)^T`. There are 23 storage-coordinate slots with one original centered-simplex coordinate constraint.
- **Chosen hypothetical complete weighted graph:** equal unit scalar masses and edge weights `w_ij=R²/d_ij²`. The weighted graph Laplacian has model eigenvalue **27/2 with exact multiplicity 16**, and **13 with exact multiplicity 4**. These dimensionless numbers are not empirically measured frequencies.
- Two separately implemented exact symbolic/rational programs reproduce **351/351** labelled distances, the predecessor values, Gram rank and eigenvalue multiplicities. Four deliberately invalid variants are detected.

## Reproducibility

```sh
python -m pip install sympy==1.14.0
python src/verify_d22.py
python tests/independent_d22.py
```

The independent checker builds all 351 squared distances from rational rules and **does not import any geometric coordinate generator**. `prior/` contains code and certificates copied from the immutable `Topbrutus/polybrutus-d21@v0.1.0`, scientific commit `f17e4d02f7442d18cdafbcbb0b62380c557e4ef2`.

Repository deliverables: `src/verify_d22.py`, `tests/independent_d22.py`, `results/certificate_d22.json` with all 351 labelled pairs, `SPECIFICATION_D22.md`, `PREUVE_D22.md`, `PROVENANCE.md`, `publication/POLYBRUTUS_22D_NOTE.pdf` and `.md`, GitHub Actions, `SHA256SUMS.txt`.

**Frozen parent DOI:** [10.5281/zenodo.24409527](https://doi.org/10.5281/zenodo.24409527).  
**Code:** MIT. **Research manuscript:** CC BY 4.0.

**Scientific limits:** Euclidean orthogonal extension and uniform graph joins are established mathematical techniques. This is a reproducible **specific synthetic metric**, not a newly discovered physical 22-dimensional spacetime, experimentally observed resonance, or novel universal theorem.
