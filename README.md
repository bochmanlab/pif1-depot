# PIF1 Family Depot (prototype)

Static site collecting sequence, structure, alleles, interactions, and literature for PIF1-family helicases.
Current entries: 21 reviewed (Swiss-Prot) members of PANTHER family PTHR47642 from animals, fungi, trypanosomes, bacteria, and phage T4 (see the About page).

- `scripts/fetch_data.py` — pulls from UniProt, AlphaFold DB, IntAct, SGD, ClinVar, PubMed into `data/`
- `scripts/build_site.py` — generates all HTML from `data/` (standard library only)
- `.github/workflows/refresh-data.yml` — weekly refresh + rebuild

To add a protein: add an entry (UniProt accession, slug, PubMed query) to `PROTEINS` in `fetch_data.py`, then run both scripts.
