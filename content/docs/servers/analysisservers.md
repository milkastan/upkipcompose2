---
title: "Analysis Servers"
date: 2021-05-20T15:51:19+03:00
draft: false
weight: 25
---

**Purpose:** Analysis servers are in the cloud platform. **Analysis servers** are configured in Microsoft Azure as **Function App**. They take the information from Influx DB or Configuration DB and make different calculations (as OEE, utilization, etc.)

Precondition: Log in **Upkip Administration** with Microsoft user. Select **Organization**.

Select menu **Analysis servers.**

- There is opened form with list of **Analysis Servers**.   Clicking on analysis server (2) is opened list of implemented Analysers (3). They are implemented in azure as Function App. 

![](/images/Aspose.Words.0026e4dc-4cb1-409d-91ad-eda9ac21484a.003.png)

*Figure 156: Upkip Administration - Analysis servers*

Select in the azure portal **All services>Function App** and filter by analyser (2).

- There are listed all function app for different analysers.

There are developed the following Analysers:

- Alarm Analyzer
- Downtime Analyzer
- Data Summary Analyzer
- Service Health Analyzer
- OEE Analyzer
- Time series Context Analyzer
- Order Analyzer
- Report Analyzer
- Machine KPI Analyzer
- Calculated Tags Analyzer

![](/images/Aspose.Words.0026e4dc-4cb1-409d-91ad-eda9ac21484a.004.png)

*Figure 157: Upkip Analysers as Azure Function App*
