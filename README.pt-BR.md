[English](https://github.com/talitadalbosco/Public-Works-Macroprocess/blob/main/README.md) · **Português**

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21673019.svg)](https://doi.org/10.5281/zenodo.21673019)
[![Licença: CC BY 4.0](https://img.shields.io/badge/Licen%C3%A7a-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/deed.pt-br)

# Macroprocesso de Obras Públicas — modelos BPMN (AS-IS e TO-BE)

Modelos de processo em BPMN 2.0 que acompanham o artigo *"A Framework for Integrating BIM and ISO 19650 into the Process Management of Public Constructions"*, publicado em **Smart and Sustainable Built Environment** (Emerald Publishing).

DOI do artigo: [10.1108/SASBE-03-2026-0230](https://doi.org/10.1108/SASBE-03-2026-0230)
DOI deste conjunto: [10.5281/zenodo.21673019](https://doi.org/10.5281/zenodo.21673019) (DOI conceito; aponta sempre para a versão mais recente)
Versão atual: 1.1.0 — ver [CHANGELOG.md](CHANGELOG.md)

---

## Descrição

Este repositório contém os diagramas completos em BPMN do macroprocesso que rege a contratação e o monitoramento de obras públicas educacionais entre o Fundo Nacional de Desenvolvimento da Educação (FNDE) e os municípios brasileiros.

São disponibilizados dois modelos:

- **AS-IS** — o macroprocesso no estado atual, reconstruído empiricamente a partir de observação direta, análise documental e entrevistas semiestruturadas realizadas no FNDE.
- **TO-BE** — uma proposta normativa de redesenho, que integra os requisitos de gestão da informação da ISO 19650 aos procedimentos exigidos pela Lei nº 14.133/2021.

Os diagramas simplificados publicados no artigo omitem subatividades, gateways e artefatos de informação, por questão de legibilidade. Os modelos deste repositório estão completos.

---

## Visualizadores interativos

Abrem diretamente no navegador, sem instalar nada:

- [**AS-IS — português**](https://talitadalbosco.github.io/Public-Works-Macroprocess/viewer/AS-IS_PT/)
- [**TO-BE — português**](https://talitadalbosco.github.io/Public-Works-Macroprocess/viewer/TO-BE_PT/)
- [AS-IS — inglês](https://talitadalbosco.github.io/Public-Works-Macroprocess/viewer/AS-IS_EN/)
- [TO-BE — inglês](https://talitadalbosco.github.io/Public-Works-Macroprocess/viewer/TO-BE_EN/)

---

## Conteúdo

Os modelos estão disponíveis em **dois idiomas**. As versões em inglês correspondem às descritas no artigo. As versões em português são os modelos originais de trabalho, mantidos porque os usuários a que este framework se destina — servidores do FNDE e equipes técnicas municipais — trabalham em português.

| Caminho | Descrição |
|---|---|
| `bpmn/AS-IS_EN/` | Macroprocesso atual, BPMN 2.0 XML (ISO 19510), inglês — um arquivo por processo (P00–P26) e por subprocesso (SP1, SP3, SP4, SP5) |
| `bpmn/AS-IS_PT/` | Macroprocesso atual, BPMN 2.0 XML (ISO 19510), português — mesma estrutura |
| `bpmn/TO-BE_EN/` | Macroprocesso proposto, BPMN 2.0 XML (ISO 19510), inglês — mesma estrutura |
| `bpmn/TO-BE_PT/` | Macroprocesso proposto, BPMN 2.0 XML (ISO 19510), português — mesma estrutura |
| `source_Nativo Bizagi/` | Arquivos nativos do Bizagi Modeler (`.bpm`, formato proprietário), cópias de arquivamento |
| `viewer/` | Visualizadores interativos em HTML, quatro combinações de modelo e idioma |

Os códigos de etapa, processo e subprocesso (`S1`–`S6`, `P01`–`P26`, `SP1`–`SP8`) são idênticos nas duas versões linguísticas, o que permite a leitura em paralelo.

**Formatos.** Os arquivos `.bpmn` da pasta `bpmn/` são o artefato principal: XML puro em conformidade com a BPMN 2.0 (ISO 19510), que pode ser aberto em qualquer ferramenta de modelagem compatível — Bizagi Modeler, Camunda Modeler, bpmn.io, Signavio, entre outras. A escolha do formato aberto é deliberada: os modelos foram feitos para serem inspecionados, adaptados e estendidos, não apenas visualizados.

Os arquivos `.bpm` da pasta `source_Nativo Bizagi/` são os originais nativos do Bizagi Modeler. Exigem software proprietário e são incluídos apenas como cópias de arquivamento, preservando documentação ou formatação específicas da ferramenta que possam não sobreviver à exportação para BPMN 2.0 XML. A reutilização deve partir da pasta `bpmn/`.

---

## Estrutura dos modelos

O macroprocesso está organizado em seis etapas, vinte e seis processos e oito subprocessos legais.

### Etapas

| Código | Etapa |
|---|---|
| S1 | Concepção e planejamento |
| S2 | Contratação pública de projeto |
| S3 | Desenvolvimento dos projetos |
| S4 | Contratação pública da execução da obra |
| S5 | Execução e monitoramento da obra |
| S6 | Encerramento |

### Processos

`P01`–`P26`, distribuídos pelas seis etapas. As responsabilidades são atribuídas a cinco categorias de agentes: FNDE, municípios, licitantes, empresas contratadas e a empresa supervisora contratada pelo FNDE.

### Subprocessos legais

`SP1`–`SP8` agrupam os procedimentos exigidos pela Lei nº 14.133/2021. Só os que têm fluxo interno próprio foram modelados como subprocessos colapsados: SP1 (DFD), SP3 (ETP), SP4 (análise de riscos) e SP5 (termo de referência). O SP2 (designação da equipe de planejamento) é uma tarefa no P04, e SP6 a SP8 aparecem como atividades numeradas (6.x, 7.x e 8.x) nos processos de seleção, contratação, fiscalização e encerramento.

---

## Reutilização

Publicado sob licença [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.pt-br). É permitido compartilhar e adaptar os modelos, inclusive para fins comerciais, desde que seja dado o devido crédito.

Os modelos foram desenvolvidos para o contexto do FNDE, mas foram concebidos para serem adaptáveis a outros órgãos financiadores centrais que operem sob arranjos de governança semelhantes. A adaptação a outros regimes de contratação — os modelos tratam apenas do regime tradicional, projeto-licitação-construção — exige a revisão das etapas S2 e S4.

---

## Como citar

> Dal'Bosco Re, T., Lima, R.M. e Azenha, M. (2026), *Public works macroprocess – BPMN models (AS-IS and TO-BE)*, Zenodo, disponível em: https://doi.org/10.5281/zenodo.21673019

Cite também o artigo:

> Dal'Bosco Re, T., Lima, R.M. e Azenha, M. (2026), "A framework for integrating BIM and ISO 19650 into the process management of public constructions", *Smart and Sustainable Built Environment*, doi: 10.1108/SASBE-03-2026-0230

---

## Financiamento

*Texto oficial, mantido em inglês conforme exigido pela entidade financiadora.*

This work is financed by national funds through FCT - Foundation for Science and Technology, under grant agreement 2022.13091.BD attributed to the 1st author and DOI https://doi.org/10.54499/2022.13091.BD. This work was also supported by FCT/MCTES under the R&D Unit Institute for Sustainability and Innovation in Structural Engineering (ISISE), under the references UID/4029/2025 (https://doi.org/10.54499/UID/04029/2025), UID/PRR/04029/2025 (https://doi.org/10.54499/UID/PRR/04029/2025) and UID/PRR2/04029/2025 (https://doi.org/10.54499/UID/PRR2/04029/2025), and under the Associate Laboratory Advanced Production and Intelligent Systems ARISE under reference LA/P/0112/2020 (https://doi.org/10.54499/LA/P/0112/2020). This work was partially supported by FCT - Fundação para a Ciência e Tecnologia within the R&D Unit Project Scope UID/00319/2025 - Centro ALGORITMI (ALGORITMI/UM) https://doi.org/10.54499/UID/00319/2025.

---

## Autores

**Talita Dal'Bosco Re** (autora correspondente)
University of Minho, ISISE, ARISE, Department of Civil Engineering, Guimarães, Portugal
ORCID: [0000-0001-8684-7904](https://orcid.org/0000-0001-8684-7904) · id9834@uminho.pt

**Rui M. Lima**
University of Minho, ALGORITMI Research Centre/LASI, Department of Production and Systems, School of Engineering, Guimarães, Portugal
ORCID: [0000-0002-7991-0132](https://orcid.org/0000-0002-7991-0132) · rml@dps.uminho.pt

**Miguel Azenha**
University of Minho, ISISE, ARISE, Department of Civil Engineering, Guimarães, Portugal
ORCID: [0000-0003-1374-9427](https://orcid.org/0000-0003-1374-9427) · miguel.azenha@civil.uminho.pt
