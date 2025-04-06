# Data Engineering Portfolio Project Plan

## Plan

### Step 1: Identify Target Companies & Data Needs

Identify 2-3 industries that genuinely interest me (e.g., e-commerce, streaming, gaming, finance). Research the common types of data and challenges within those industries (e.g., user clickstreams, sales transactions, game telemetry) using LLMs, industry reports, job postings, and/or data engineering blogs. Choose a project theme based on a common, relatable dataset type that allows you to demonstrate a wide range of DE skills. This still shows industry awareness without risking analysis paralysis.

### Step 2: Find Suitable Datasets Online

- Realistic: Not perfectly clean; requires cleaning, handling missing values, different formats (CSV, JSON, etc.).
- Sufficiently Complex: Allows for joins, aggregations, and meaningful transformations.
- Appropriately Sized: Manageable for a personal project but large enough to be non-trivial (millions of rows).
- Publicly Available: E.g. Kaggle, government open data, Awesome Public Datasets on GitHub.

### Step 3: Define End Users & Use Cases

Defining _who_ the data is for (e.g., marketing team, sales analysts) and _what_ they need to do with it (e.g., analyze campaign effectiveness, track regional sales) to identify the **purpose** for the pipeline. It will guide technical decisions regarding transformations, data models, and the final dashboard.

### Step 4: Set Up Workspaces, Create Resources & Implement Pipeline with medallion architecture (Bronze/Silver/Gold)

Using Fabric components like Lakehouse, Notebooks, Dataflows/Pipelines, semantic models, BI-dashboards, etc.. The medallion architecture and final dashboards should clearly address the business problems / use-cases defined in Step 3.

### Step 5: Connect to GitHub & Set Up Repository

- A clear, detailed `README.md` explaining the project, architecture, setup, and how to view the results.
- Logical code organization.
- Good commit hygiene.

### Step 6: Set up CI/CD in Microsoft Fabric

Demonstrate CI/CD concepts using Deployment Pipelines for supported artifacts (e.g., Power BI reports), and simulate or document manual deployment steps for unsupported components.

### Step 7: Document the Final Project

- Executive summary, with a clearly defined business problem the solution seeks to fix.
- A complete list of data sources
- The purpose of the dataset
- How data integrity and quality were maintained
- Workspace assignment and reasoning.
- Snapshots of:
  - the dashboards for the different users
  - data lineage, and
  - the data pipeline (including a text summary of the ETL-automation steps)

### Step 8: Create Dashboard (Power BI Free/Public)

- Since the Fabric trial will run out eventually, migrate the gold-level semantic models to Power BI desktop, publish to Power BI Service and then select "File"> “Embed report” > “Publish to web (public)” to get a link that I can use to share my dashboard for free (alongside all underlying data, but that is not a problem as the datasets will be public anyway).
- Using Power BI Free and publishing publicly makes it easy to share in your portfolio.

### Step 9: Publish the Entire Project in my Portfolio Website, including youtube walkthrough

- The documented project summary
- The embedded Power BI report
- Links to the Github repository

Additionally, create a youtube walkthrough videos and embed the video in my portfolio.

## Open Questions

- How can I practically implement slowly changing dimensions? Maybe if I can find a fact table split up by month?
