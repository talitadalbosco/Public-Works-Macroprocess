# Changelog

## [1.1.0] — 2026-10-11

Corrections to labels, nomenclature and typographical errors in the process models. No sequence flow was added, removed or rerouted; the order of activities and the allocation of responsibilities are unchanged. Unless noted, changes apply to the four model sets (AS-IS and TO-BE, English and Portuguese).

### Changed

- The instrument between FNDE and municipalities is now named "Terms of Commitment" / "Termo de Compromisso" (formerly "Contract between FNDE and Municipalities" / "Contrato entre FNDE e Municípios") in P00 and P03; in the Portuguese TO-BE, P12 refers to the "Termo de Compromisso revisado".
- P11 and P20: the task "8.2 Receive provisionally" / "8.2 Receber provisoriamente" is renamed "Accept delivery and certify measurement" / "Atestar a entrega e a medição". Provisional receipt of the object (8.2) remains in P13 and P23.
- P21 and P24 (and P26 in the English models): "Access the proposal in the system" / "Acessar a proposta no sistema" is renamed "Access the work in the system" / "Acessar a obra no sistema".
- Project codes harmonised: "PDR MNC" → "PRJ MNC", "PDR ASB" → "PRJ ASB", "DRI 12/13 PRJ MNC" → "DRI P12/P13 PRJ MNC".
- Previously unnamed data stores are labelled: SIMEC (P02, P03, P12, P21, P22, P24), non-conformity records (P21, P24) and PAR diagnosis (P01), except in the English AS-IS; in the TO-BE models, CDE (P09, P10, P18, P19).
- Portuguese TO-BE, P05 and P14: the evaluation criteria refer to the pre-appointment BEP ("BEP pré-contratual").
- Portuguese models: process names in P00 harmonised with the diagram names (P06, P15, P22, P25).
- Portuguese typographical errors corrected: "Prestação de Contas" (P25 file and diagram name), "Análise de Risco" (SP4), "não conformidades" (P21, P24), "fornecedor" (SP5), "prioridade" (SP1), "Coordenador Nível 4".

### Added

- P23: the Final Receipt Form / Termo de Recebimento Definitivo is shown as an output of the submission to FNDE, making visible the origin of this input in P24.
- Portuguese TO-BE: P21 output "Painel de monitoramento"; P23 (5.8.1) output "Modelo para gestão do ativo".

### Repository

- Metadata file renamed from `zenodo.json` to `.zenodo.json`, so that Zenodo reads it (resource type: dataset).
- README (English and Portuguese): file paths corrected; description of the legal subprocesses corrected (only SP1, SP3, SP4 and SP5 are modelled as collapsed subprocesses); inspection enterprise added to the actor categories; stage names corrected.
- Reference to a `templates/` folder removed, as the reference documents are not distributed in this repository.
- `CITATION.cff` and `.zenodo.json` updated to version 1.1.0; `.gitignore` added.
- HTML viewers re-exported.

## [1.0.1] — 2026-07-29

Zenodo DOI added to README and CITATION.cff.

## [1.0.0] — 2026-07-29

Initial release, supplementary material to Dal'Bosco Re, Lima and Azenha (2026), *Smart and Sustainable Built Environment*, doi: 10.1108/SASBE-03-2026-0230.
