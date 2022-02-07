# Asymmetry by Design? Identity Obfuscation, Reputational Pressure, and Consumer Predation in U.S. For-Profit Higher Education

### by Adam Goldstein and Charlie Eaton

Summary: Colleges that are part of multi-brand companies invest less in instruction, have worse student outcomes, and are more likely to face legal and regulatory sanctions (relative to single-brand firms).

**Data:**
  - For-profit News Article DataHub Data
  - Private Equity and College Ownership DataHub Data
  - Borrower Defense Complaint DataHub Data
  - IPEDS Completions
  - College Scorecard
  - IPEDS Institutional Characteristics
  - IPEDS Fall Staff
  - IPEDS Graduation Rates
  - IPEDS Fall Enrollment by Race
  - IPEDS Financial Aid and Net Price

**Citatation:**
Goldstein, Adam, and Charlie Eaton. “Asymmetry by Design? Identity Obfuscation, Reputational Pressure, and Consumer Predation in U.S. For-Profit Higher Education.” American Sociological Review 86, no. 5 (October 2021): 896–933. https://doi.org/10.1177/00031224211043223.

**Abstract:**
This article develops and tests an identity-based account of malfeasance in consumer markets. We hypothesize that multi-brand organizational structures help predatory firms short-circuit reputational discipline by rendering their underlying identities opaque to consumer audiences. The analysis utilizes comprehensive administrative data on all U.S. for-profit colleges, an industry characterized by widespread fraud and poor (although variable) educational outcomes. Consistent with the hypothesis that brand multiplicity facilitates malfeasance by reducing ex ante reputational risks, colleges that are part of multi-brand companies invest less in instruction, have worse student outcomes, and are more likely to face legal and regulatory sanctions (relative to single-brand firms). Maintaining multiple outward-facing brand identities also mitigates reputational penalties in the wake of law enforcement actions, as measured by news coverage of legal actions, and by subsequent enrollment growth. The results suggest identity multiplicity plays a key role in allowing firms to furnish substandard products, even amid frequent scandals and media scrutiny. Predatory practices are facilitated not only by the inherent informational asymmetries in a given product, but also by firms’ efforts to make themselves less legible to audiences. The analysis contributes to research on higher education, organizational theory, and the sociology of markets.

**Using the Code and Data:**
If you cannot use Git to clone this package to your machine, you can download all files and folders in the package by clicking on the green **Code** button at the top of this page. Alternatively, if you navigate to any program or data file in the repository above using your web browser, there will be a **download** button on the bottom right of your browser page to download that individual file.

All replication code is in STATA but is provided and executed in Jupyter Notebooks (.ipnynb) using a Stata Kernel. For details see: https://kylebarron.dev/stata_kernel/

Each .ipynb Notebook file begininning with "f" in the repository includes both code for producing figures in the paper and a rendering of the given table figure. Notebook "f1" corresponds to "Figure 1" in the paper and so on. Notebook "fa1" corresponds to "Figure A1" in the online appendix and so on. 

Each .ipynb Notebook file begininning with "t" in the repository includes both code for producing tables in the paper and a rendering of given table. As with figures, Notebook "t3" corresponds to "Table 3" in the paper and so on. There are no replication Notebooks for Table 1, Table 2, or Appendix Table A1 because they were produced by hand in a spreadsheet.

Each figure and table Notebook includes a code cell with STATA code for downloading from this repository the particular datasets used for the given figure or table. If you have already cloned the entire repository or otherwise downloaded the dataset, we recommend commenting out or otherwise skip the code cell for downloading the data. This will make the replication code execute much faster. Relatedly, if you do not use Jupyter Notebooks, you can simply use control C within your web browser to copy all of the code in any Notebook link and then paste the code into a STATA .do file to execute.

The .ipynb files beginning with "d" build datasets for our analyses from source datasets. If you want to see how we identify multi-brand firms and campuses, you should particularly see the d_codemultibrandunitid.ipynb Notebook. We also explain how the multi-brand encoding works in the Online Appendix. Source datasets and datasets used for analyses in the paper are in the **data** folder above. Note, if you run the code to build the datasets from source data and use the output datasets with our figure and table replication Notebooks above, results will be substantively equivalent and robust but will not replicate exactly for sales employees, law enforcement actions, earnings, or brand news article models in Tables 3, 7, and 8. This is because these dependent variables are measured and modeled at the firm and OPEID level, requiring the collapsing and coding of modal school-level categorical control variables (such as the state in which a school is located) at a higher organizational level. When STATA sorts and collapses such categorical control variables, it breaks ties in modal categorical values randomly when running the same sort repeatedly. This is explained by William Gould of StataCorp [here](https://www.stata.com/support/faqs/programming/sorting-on-categorical-variables/).

The "figures" directory of the repository above contains .pdf outputs of each figure in the paper. The "tables" directory includes .rtf outputs of each table in the paper. Please feel to contact us with any questions about the paper or the replication package via the "issues" tab above.
