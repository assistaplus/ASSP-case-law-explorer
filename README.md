# Case Law Explorer

Materials for building a network analysis software platform for analyzing Dutch and European court decisions. This repository builds on the work by Dafne van Kuppevelt of the Netherlands e-Science Centre [NLeSC/case-law-app](https://github.com/NLeSC/case-law-app).

## Quickstart

- Setup and run locally the extraction pipeline with the [Caselaw extraction walkthrough](https://maastrichtlawtech.github.io/case-law-explorer/#/etl/)
- Setup and run a GraphQL API with AWS in the [GraphQL API walkthrough](https://maastrichtlawtech.github.io/case-law-explorer/#/graphql/)

## Datasets

See [Datasets](/datasets/). Currently, we gather the case law of the Netherlands and that of two European courts, as it follows:

- **Published and operable**
    - [Rechtspraak](https://maastrichtlawtech.github.io/case-law-explorer/#/datasets/?id=rechtspraak-archive), backed by [Legal Intelligence](https://maastrichtlawtech.github.io/case-law-explorer/#/datasets/?id=legal-intelligence-api), and citations provided by [LIDO](https://maastrichtlawtech.github.io/case-law-explorer/#/datasets/?id=linked-data-overheid-lido)
- **Work in progress**
    - [European Court of Human Rights](https://maastrichtlawtech.github.io/case-law-explorer/#/datasets/?id=european-court-of-human-rights-echr) with WIP scripts available on [GitHub](https://github.com/maastrichtlawtech/case-law-explorer/blob/master/data_extraction/caselaw/echr/ECHR_metadata_harvester.py) 
    - [Court of Justice of the European Union](https://maastrichtlawtech.github.io/case-law-explorer/#/datasets/?id=court-of-justice-of-the-european-union-cjeu) with WIP scripts available on [GitHub](https://github.com/maastrichtlawtech/case-law-explorer/blob/master/data_extraction/caselaw/cellar/cellar_extraction.py)

We plan to extend the data to other international courts.

## Taxonomy

Proceeding into this documentation, there will be multiple legal or structural terms used. They are defined over here.

|                 Term                |                                         Definition                                        |
|:-----------------------------------:|:-----------------------------------------------------------------------------------------:|
| ECLI (European Case Law Identifier) | Unique identifier for court decisions in Europe                                           |
| Issued date                         | Date of document publication                                                              |
| Enactment Date                      | Date of court decision                                                                    |
| Language                            | Language of jurisdiction to which case belongs                                            |
| Creator                             | Name of instance (court)                                                                  |
| Zaaknummer                          | Case number, for internal use by courts                                                   |
| Case type                           | 'uitspraak' (decision) or 'conclusie' (opinion)                                           |
| Procedure type                      | e.g. summary proceedings                                                                  |
| Spatial                             | Court location (municipality)                                                             |
| Subject                             | Domain (area of the law) applicable to case                                               |
| Relation                            | Predecessor and successor cases (in case of appeal, cassation, preliminary decisions etc) |
| References                          | Title of applicable legislation                                                           |
| Inhoudsindicatie                    | Case summary                                                                              |

## Contributors

<!-- readme: contributors,gijsvd -start -->
<!-- readme: contributors,gijsvd -end -->

## License 

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

Previously under the [Creative Commons Attribution-NonCommercial 4.0 International](https://creativecommons.org/licenses/by-nc/4.0/legalcode.en)), as of 13/02/2022 this work is licensed under a [MIT License](https://opensource.org/licenses/MIT).

```
MIT License

Copyright (c) 2022 Maastricht Law & Tech Lab

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
