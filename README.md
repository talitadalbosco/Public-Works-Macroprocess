**English** · [Português](README.pt-BR.md)

# Public Works Macroprocess — BPMN models (AS-IS and TO-BE)

BPMN 2.0 process models supporting the article *"A Framework for Integrating BIM and ISO 19650 into the Process Management of Public Constructions"*, published in **Smart and Sustainable Built Environment** (Emerald Publishing).

Article DOI: [10.1108/SASBE-03-2026-0230](https://doi.org/10.1108/SASBE-03-2026-0230)

---

## Description

This repository contains the complete Business Process Model and Notation (BPMN) diagrams of the macroprocess governing the contracting and monitoring of educational public works between the Brazilian National Fund for Education Development (FNDE) and municipalities.

Two models are provided:

- **AS-IS** — the current-state macroprocess, empirically reconstructed from direct observation, document analysis and semi-structured interviews conducted at FNDE.
- **TO-BE** — a normative redesign integrating ISO 19650 information management requirements with the procedures mandated by Brazilian Public Procurement Law No. 14,133/2021.

The simplified diagrams published in the article omit sub-activities, gateways and information artefacts for legibility. The models in this repository are complete.

---

## Contents

Models are provided in **two languages**. The English models correspond to the version described in the article. The Portuguese models are the original working versions, retained because the intended users of this framework — FNDE staff and Brazilian municipal technical teams — work in Portuguese.

| Path | Description |
|---|---|
| `bpmn/AS-IS_EN.bpmn` | Current-state macroprocess, BPMN 2.0 XML (ISO 19510), English |
| `bpmn/AS-IS_PT.bpmn` | Current-state macroprocess, BPMN 2.0 XML (ISO 19510), Portuguese |
| `bpmn/TO-BE_EN.bpmn` | Proposed macroprocess, BPMN 2.0 XML (ISO 19510), English |
| `bpmn/TO-BE_PT.bpmn` | Proposed macroprocess, BPMN 2.0 XML (ISO 19510), Portuguese |
| `source/*.bpm` | Native Bizagi Modeler files (proprietary), archival copies |
| `viewer/AS-IS_EN/` · `viewer/AS-IS_PT/` | Interactive HTML viewer, AS-IS |
| `viewer/TO-BE_EN/` · `viewer/TO-BE_PT/` | Interactive HTML viewer, TO-BE |
| `templates/` | Reference information requirement documents (F_EIR, example EIR and BEP) |

Interactive viewers are served at `https://talitadalbosco.github.io/Public-Works-Macroprocess/viewer/<MODEL>_<LANG>/`

Stage, process and subprocess codes (`S1`–`S6`, `P01`–`P26`, `SP1`–`SP8`) are identical across both language versions, so the models can be read in parallel.

**Formats.** The `.bpmn` files in `bpmn/` are the primary artefact: plain XML conforming to BPMN 2.0 (ISO 19510), openable in any compliant modelling tool — Bizagi Modeler, Camunda Modeler, bpmn.io, Signavio, among others. They are provided in an open format deliberately: the models are intended to be inspected, adapted and extended, not only viewed.

The `.bpm` files in `source/` are the native Bizagi Modeler originals. They require proprietary software and are included only as archival copies, preserving any tool-specific documentation or formatting that may not survive export to BPMN 2.0 XML. Reuse should start from `bpmn/`.

---

## Model structure

The macroprocess is organised into six stages, twenty-six processes and eight legal subprocesses.

### Stages

| Code | Stage |
|---|---|
| S1 | Conception and planning |
| S2 | Public procurement of design services |
| S3 | Design development |
| S4 | Public tender of works execution |
| S5 | Execution and monitoring of the work |
| S6 | Closing |

### Processes

`P01`–`P26`, distributed across the six stages. Responsibility is allocated to four actor categories: FNDE, municipalities, prospective enterprises and enterprises.

### Legal subprocesses

`SP1`–`SP8` group the procedures required by Law No. 14,133/2021, modelled as collapsed subprocesses embedded in the macroprocess.

---

## Reuse

Released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You may share and adapt the models, including for commercial purposes, provided appropriate credit is given.

The models were developed for the FNDE context but are intended to be adaptable to other central funding bodies operating under comparable governance arrangements. Adaptation to different procurement arrangements — the models address Design-Bid-Build only — requires revision of stages S2 and S4.

---

## How to cite

> Dal'Bosco Re, T., Lima, R.M. and Azenha, M. (2026), *Public Works Macroprocess — BPMN models (AS-IS and TO-BE)* [Data set], Zenodo, doi: 10.5281/zenodo.XXXXXXX

Please cite the article as well:

> Dal'Bosco Re, T., Lima, R.M. and Azenha, M. (2026), "A framework for integrating BIM and ISO 19650 into the process management of public constructions", *Smart and Sustainable Built Environment*, doi: 10.1108/SASBE-03-2026-0230

---

## Funding

This work is financed by national funds through FCT - Foundation for Science and Technology, under grant agreement 2022.13091.BD attributed to the 1st author and DOI https://doi.org/10.54499/2022.13091.BD. This work was also supported by FCT/MCTES under the R&D Unit Institute for Sustainability and Innovation in Structural Engineering (ISISE), under the references UID/4029/2025 (https://doi.org/10.54499/UID/04029/2025), UID/PRR/04029/2025 (https://doi.org/10.54499/UID/PRR/04029/2025) and UID/PRR2/04029/2025 (https://doi.org/10.54499/UID/PRR2/04029/2025), and under the Associate Laboratory Advanced Production and Intelligent Systems ARISE under reference LA/P/0112/2020 (https://doi.org/10.54499/LA/P/0112/2020). This work was partially supported by FCT - Fundação para a Ciência e Tecnologia within the R&D Unit Project Scope UID/00319/2025 - Centro ALGORITMI (ALGORITMI/UM) https://doi.org/10.54499/UID/00319/2025.

---

## Authors

**Talita Dal'Bosco Re** (corresponding author)
University of Minho, ISISE, ARISE, Department of Civil Engineering, Guimarães, Portugal
ORCID: [0000-0001-8684-7904](https://orcid.org/0000-0001-8684-7904) · id9834@uminho.pt

**Rui M. Lima**
University of Minho, ALGORITMI Research Centre/LASI, Department of Production and Systems, School of Engineering, Guimarães, Portugal
ORCID: [0000-0002-7991-0132](https://orcid.org/0000-0002-7991-0132) · rml@dps.uminho.pt

**Miguel Azenha**
University of Minho, ISISE, ARISE, Department of Civil Engineering, Guimarães, Portugal
ORCID: [0000-0003-1374-9427](https://orcid.org/0000-0003-1374-9427) · miguel.azenha@civil.uminho.pt
