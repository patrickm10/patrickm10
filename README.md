<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=26&duration=3000&pause=800&color=36BCF7&center=true&vCenter=true&width=700&lines=Patrick+Mejia+%7C+Data+Engineer;Pipelines+%E2%86%92+Warehouses+%E2%86%92+Products;Dagster+%C2%B7+Airflow+%C2%B7+BigQuery+%C2%B7+dbt;Millions+of+records%2C+every+day." alt="Typing SVG" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/patrick-mejia-6045151a1)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:pmejia1010@gmail.com)
[![PEM Sports](https://img.shields.io/badge/PEM_Sports-live-2ea44f?style=flat-square&logo=vercel&logoColor=white)](https://www.pemsports.com)
![Location](https://img.shields.io/badge/Boston,_MA-555?style=flat-square&logo=googlemaps&logoColor=white)

</div>

---

### `$ cat profile.yaml`

```yaml
engineer:
  name: Patrick Mejia
  role: Data Engineer / Analyst @ Warren Rogers
  location: Boston, MA
  languages: [English, Spanish]

focus:
  - cloud-native data platforms
  - ETL/ELT pipelines & orchestration
  - data quality, testing & governance
  - turning raw telemetry into decisions

education:
  - { school: WPI, degree: M.S. Computer Science, status: in_progress, expected: 2027 }
  - { school: WPI, degree: B.S. Computer Science, year: 2023, honors: Distinction }

certifications:
  - Astronomer DAG Authoring
  - Astronomer Airflow Fundamentals

currently_shipping: pemsports.com
sla: reply within 24h  # say hi 👋
```

---

### `SELECT * FROM career ORDER BY start_date DESC;`

| company | role | stack | impact |
|---|---|---|---|
| **Warren Rogers** | Data Engineer / Analyst | Dagster · SQL · SAS · Power BI | Ingests **millions** of minute-level sensor readings/day from **3,000+** sites for 24/7 inventory reporting |
| **PEM Sports** | Founder & Lead Engineer | React · FastAPI · Supabase · GitHub Actions | Live NFL analytics platform; ingestion automation cut manual effort **>90%** |
| **Iron Mountain** | Data Platform Engineer | GCP · BigQuery · Airflow · Terraform · Jenkins | Self-service data onboarding platform adopted by **30+** teams; **+20%** pipeline automation |
| **Laronde** | Software Engineer Intern | Python · BioPython · BigQuery | Parsed **2,000+** GenBank files into a queryable genomic database |
| **Advanced Instruments** | Engineering Intern | Python · PyQt · SQL | Redesigned an osmometer UI; built a compliance-tracking database |

<sub>`5 rows returned` · `query time: 2019 → present`</sub>

---

### 🏈 Featured: [PEM Sports](https://www.pemsports.com) architecture

A production NFL analytics platform I designed, built, and operate end to end. It covers 800+ players, teams, seasons, and matchups.

```mermaid
flowchart LR
    subgraph Ingest
        A[NFL data sources] --> B[Python / Pandas<br/>ingestion jobs]
    end
    subgraph Store
        B --> C[(Supabase<br/>PostgreSQL)]
    end
    subgraph Model
        C --> D[Normalized schemas<br/>& SQL views]
        D --> E[Linear & Poisson<br/>regression projections]
    end
    subgraph Serve
        D --> F[FastAPI on Render]
        E --> F
        F --> G[React on Vercel]
    end
    H[GitHub Actions CI<br/>tests · validation · releases] -.-> B
    H -.-> F
    H -.-> G
```

---

### 🛰️ What I build at work: sensor telemetry at scale

```mermaid
flowchart LR
    S[3,000+ fuel-station sites<br/>minute-level sensors] --> P[Dagster pipelines<br/>daily & monthly]
    P --> V{SQL / SAS<br/>validation checks}
    V -- missing · dupes · spikes · temp anomalies --> AL[Anomaly alerts]
    V -- clean --> R[24/7 inventory<br/>reporting]
    AL --> GT[Ground-truth fault labels<br/>for future ML detection]
    R --> BI[Power BI<br/>site & state views]
```

---

### 🧱 Stack by pipeline layer

| Layer | Tools |
|---|---|
| **Ingest** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Pub/Sub](https://img.shields.io/badge/Pub%2FSub-4285F4?style=flat-square&logo=googlecloud&logoColor=white) ![Cloud Functions](https://img.shields.io/badge/Cloud_Functions-4285F4?style=flat-square&logo=googlecloud&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) |
| **Orchestrate** | ![Dagster](https://img.shields.io/badge/Dagster-4F43DD?style=flat-square&logo=dagster&logoColor=white) ![Airflow](https://img.shields.io/badge/Apache_Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white) |
| **Transform** | ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white) ![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white) ![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white) ![SAS](https://img.shields.io/badge/SAS-0766D1?style=flat-square) |
| **Store** | ![BigQuery](https://img.shields.io/badge/BigQuery-669DF6?style=flat-square&logo=googlebigquery&logoColor=white) ![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white) ![S3](https://img.shields.io/badge/AWS_S3-569A31?style=flat-square&logo=amazons3&logoColor=white) |
| **Quality & Governance** | ![Great Expectations](https://img.shields.io/badge/Great_Expectations-FF6310?style=flat-square) ![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white) ![IAM](https://img.shields.io/badge/IAM_&_Policy_Tags-4285F4?style=flat-square&logo=googlecloud&logoColor=white) |
| **Infra & CI/CD** | ![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=flat-square&logo=terraform&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white) |
| **Serve & Visualize** | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) |

---

### 📈 Observability (aka my GitHub metrics)

<div align="center">
  <img height="165" alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=patrickm10&show_icons=true&hide=issues,contribs&hide_border=true&theme=tokyonight" />
  <img height="165" alt="Top languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=patrickm10&layout=compact&hide_border=true&theme=tokyonight" />
</div>

---

<div align="center">

```text
[pipeline] status=healthy · last_run=today · next_run=tomorrow 06:00 · open_to=collaboration
```

</div>
