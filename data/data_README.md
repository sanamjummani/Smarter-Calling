# Data

## Dataset — Portuguese Bank Marketing Campaign

The dataset used in this analysis is the **Bank Marketing dataset** collected by a Portuguese banking institution between May 2008 and November 2010, covering direct phone-based marketing campaigns for term deposit subscriptions.

It is publicly available via the **UCI Machine Learning Repository**, one of the most widely used sources for academic machine learning datasets.

### What it contains

| Field | Type | Description |
|---|---|---|
| `age` | numeric | Customer age |
| `job` | categorical | Employment type |
| `marital` | categorical | Marital status |
| `education` | categorical | Education level |
| `default` | categorical | Has credit in default? |
| `housing` | categorical | Has housing loan? |
| `loan` | categorical | Has personal loan? |
| `contact` | categorical | Contact communication type |
| `month` | categorical | Last contact month |
| `day_of_week` | categorical | Last contact day |
| `pdays` | numeric | Days since last contacted in prior campaign |
| `previous` | numeric | Number of prior campaign contacts |
| `poutcome` | categorical | Outcome of previous campaign |
| `emp.var.rate` | numeric | Employment variation rate (economic indicator) |
| `cons.price.idx` | numeric | Consumer price index (economic indicator) |
| `cons.conf.idx` | numeric | Consumer confidence index |
| `euribor3m` | numeric | Euribor 3 month rate |
| `nr.employed` | numeric | Number of employees (economic indicator) |
| `y` | binary | **Target — did the customer subscribe?** (yes / no) |

**41,188 records** in the raw dataset · **5,466 records** after cleaning

### Why it is not included here

The dataset file is not included in this repository. The data is publicly available and free to download directly from its source.

To reproduce the analysis, download the file from the UCI ML Repository and place it in this folder:

[https://archive.ics.uci.edu/dataset/222/bank+marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing)

Download `bank-additional-full.csv`, place it in this folder, and rename it `targeted-telemarketing.csv`. The notebook will run without any other changes.

### Citation

Moro, S., Cortez, P., & Rita, P. (2014). A data-driven approach to predict the success of bank telemarketing. *Decision Support Systems*, 62, 22–31.
