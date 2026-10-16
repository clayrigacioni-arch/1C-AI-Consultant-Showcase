**English** | [Русский](README_RU.md) | [Azərbaycan dili](README_AZ.md)

# AI Consultant for 1C:Enterprise — v3

AI Consultant helps users retrieve analytical reports in 1C through natural-language questions. It supports questions in **Russian and Azerbaijani**.

The project has reached its **third product version**. The current demo uses standard 1C reports and the Data Composition System (DCS).

## What changed in v3

The project has evolved from analytical query generation and custom visualization to configuring standard reports.

AI identifies the user’s task and report parameters: period, groupings, filters, and metrics. The application validates these against the available scenario catalog and applies them to a configured report variant. Calculations and report generation run through 1C.

A shared scenario-processing mechanism allows the solution to grow by connecting and configuring additional reports.

## Demo capabilities

- Sales analysis by customer, product, and organization.
- Purchasing analysis by supplier and product.
- Inventory movement analysis by warehouse and product.
- Report configuration through natural-language questions.
- Processing of Russian and Azerbaijani requests.

Example questions in the supported languages:

- “Покажи выручку за 2024 год по клиентам и номенклатуре”.
- “2024-cü il üzrə müştərilər və məhsullar üzrə satış gəlirini göstər”.
- “2023-cü ildə təchizatçılar üzrə alışları göstər”.
- “Anbarlar üzrə mal hərəkətini göstər”.

## Current status

Available capabilities depend on the reports and report variants configured in each 1C database. Testing, expansion of analytical scenarios, and improvements to cash-flow reporting are ongoing. Support for more complex analytical requests is planned.

Technologies: 1C:Enterprise 8.3, BSL, DCS, standard reports, OpenAI API, HTTP/JSON.

This repository contains the public product description and demonstration materials. Source code, distribution files, and internal AI instructions are not published.

## v3 demo: question → report

Screenshots from the demonstration database show a natural-language question followed by the resulting standard 1C report.

### Warehouse movements — Azerbaijani question

Question: “anbarlar üzrə mal hərəkətini göstər 2023-cü il üzrə”.

![Warehouse movement question in Azerbaijani](screenshots/v3/warehouse-question-az.jpg)

Result: the warehouse report for 01.01.2023–31.12.2023, showing opening balance, receipts, issues, and closing balance.

![Warehouse movement report for 2023](screenshots/v3/warehouse-report.jpg)

### Purchasing analysis — Russian question

Question requesting purchase amounts for 2022 by supplier and product.

![Purchasing analysis question in Russian](screenshots/v3/purchases-question-ru.jpg)

Result: the purchasing report for 01.01.2022–31.12.2022, grouped by supplier and product.

![Purchasing report for 2022 by supplier and product](screenshots/v3/purchases-report.jpg)

## Screenshots from previous versions

The following images show the interface and visualization features of previous product versions. They are not v3 screenshots. The materials were created using a demonstration database.

![Previous version overview](github-social-preview.jpg)

![Previous version interface](main-interface.jpg)

![Table in a previous version](table-result.jpg)

![Chart in a previous version](chart-result.jpg)

![Graph in a previous version](graph-result.jpg)
