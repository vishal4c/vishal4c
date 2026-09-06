<div align="center">

<img src="./assets/banner.svg" alt="Vishal Kumar: geospatial AI, big spatial data, maps and routing systems" width="100%">

<br>

<img src="./assets/headshot.png" alt="Vishal Kumar" width="170">

# Vishal Kumar

### Geospatial AI, big spatial data, and the systems that turn open data into maps and routes.

<img src="https://readme-typing-svg.demolab.com?font=Inter&weight=600&size=22&duration=2800&pause=900&color=0F766E&center=true&vCenter=true&width=900&lines=Agentic+AI+and+vision-language+models+for+map+editing;Planet-scale+spatial+pipelines%3A+Spark%2C+Sedona%2C+Planetiler%2C+GeoParquet;Map+conflation%2C+routing+networks%2C+GPS+trajectory+ML;OpenStreetMap%2C+Overture+Maps%2C+open+geospatial+tooling" alt="Research themes" width="92%">

<p>
  <a href="https://www.linkedin.com/in/vishalnitt/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-vishalnitt-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"></a>
  <a href="https://dl.acm.org/doi/10.1145/3557991.3567784"><img alt="ACM DL" src="https://img.shields.io/badge/ACM%20DL-SIGSPATIAL-0F766E?style=for-the-badge&logo=acm&logoColor=white"></a>
  <a href="https://hackernoon.com/u/vishalkumar"><img alt="HackerNoon" src="https://img.shields.io/badge/HackerNoon-Articles-00FE00?style=for-the-badge&logo=hackernoon&logoColor=black"></a>
  <a href="https://www.youtube.com/watch?v=N96IdetD6CE"><img alt="Talk" src="https://img.shields.io/badge/Talk-SotM%20US%202026-FF0000?style=for-the-badge&logo=youtube&logoColor=white"></a>
  <a href="mailto:vishku@amazon.com"><img alt="Email" src="https://img.shields.io/badge/Email-vishku%40amazon.com-0F172A?style=for-the-badge&logo=gmail&logoColor=white"></a>
</p>

</div>

I am a Senior Software Engineer and Tech Lead at Amazon Last Mile Maps in Seattle. I own the architecture of Amazon's map-making stack: the big-data pipelines that produce the routable road network behind millions of daily delivery routes, and the planet-scale tile generation built on the OpenStreetMap toolchain. My current research applies LLM and vision-language agents to map editing, conflation, and geospatial data labeling, with deterministic verifiers that check every agent edit before it reaches the map.

## Research interests

| Area | What I work on |
| --- | --- |
| Agentic AI for geospatial tasks | Agent harnesses for map editing, tool-grounded reasoning over satellite and street-view imagery, verifier-in-the-loop labeling, multi-agent critic loops. |
| Big spatial data systems | Planet-scale ETL on Spark and Apache Sedona, database-free vector tile generation (Planetiler, GeoParquet, PMTiles), incremental map updates. |
| Map conflation and migration | Cross-provider road correspondence, geometric edit replay, transferring private edits between OpenStreetMap and Overture base maps. |
| Trajectory and sensor ML | Driver-activity classification from raw GPS traces, ground-truth aggregation from fleet telemetry, GNSS-based building entry detection. |
| Intelligent transportation | Routing networks for last-mile and pedestrian delivery, entrance and access-point extraction, sidewalk and walk-path detection. |

## Publications

**2026**

- **Scalable Conflation for Maps Data Replay between Heterogeneous Geospatial Data Sources.**
  ACM SIGSPATIAL 2026, Industrial Track. Seattle, Nov 2026.
  [Accepted papers](https://sigspatial2026.sigspatial.org/industry-accepted/)
- **MapScout: An Agentic Harness for Map Editing and Geospatial Data Labeling.**
  ACM SIGSPATIAL 2026, Demonstration Track. Seattle, Nov 2026.
  [Accepted demos](https://sigspatial2026.sigspatial.org/demo-accepted/)

**2022**

- **Deep Classification of Frequently-Changing Activities from GPS Trajectories.**
  ACM SIGSPATIAL Workshop on Computational Transportation Science (IWCTS 2022).
  [DOI 10.1145/3557991.3567784](https://doi.org/10.1145/3557991.3567784)
  The model replaced heuristic driver-activity inference across Amazon's worldwide delivery operations. Companion open dataset: [GOAL: GPS Ordered Activity Labels](https://github.com/amazon-science/goal-gps-ordered-activity-labels).

## Talks and workshops

| When | Venue | Title |
| --- | --- | --- |
| Nov 2, 2026 | FOSS4G North America 2026, Sacramento | Workshop: [Routes to Safety: A Wildfire Evacuation Map from Open Data](https://talks.osgeo.org/foss4g-na-2026/talk/NYKALL/), with Shaishav Maisuria. Materials: [vishal4c/routes-to-safety-workshop](https://github.com/vishal4c/routes-to-safety-workshop) |
| Nov 4, 2026 | ACM SIGSPATIAL 2026, Seattle | Presenting the Scalable Conflation paper and the MapScout demo |
| Jun 12, 2026 | State of the Map US 2026, Madison | [How Amazon Generates Map Tiles for Last-Mile Delivery Using OSM-Derived Datasets and Planetiler](https://openstreetmap.us/events/state-of-the-map-us/2026/how-amazon-generates-map-tiles/) ([video](https://www.youtube.com/watch?v=N96IdetD6CE)) |
| Oct 2022 | ACM SIGSPATIAL IWCTS 2022, Seattle | Deep Classification of Frequently-Changing Activities from GPS Trajectories |

## Systems in Production

- **FlashTileGenEngine.** Database-free vector tile pipeline (Planetiler, GeoParquet, Apache Sedona on Spark) that replaced a PostGIS stack. Worldwide tile refresh dropped from 31 hours to 4, 22 logistics-specific layers, tiles served across 19 countries.
- **Routable road network generation.** Big-data pipeline (2019) that builds Amazon's last-mile road graph; later Spark migration took world-wide map ingestion from a 48-hour monolith to an 8-hour distributed job.
- **GeoAI agent framework.** Multi-agent system on AWS Bedrock AgentCore with 22 production tools and 10 sub-agents for geospatial analysis, reaching 1,000+ internal partners.
- **Driver activity classifier.** Bi-directional LSTM with attention that infers activity from GPS traces alone, in production worldwide since 2024. Its outputs feed Amazon's driver-safety analytics ([About Amazon, Sept 2025](https://www.aboutamazon.com/news/transportation/amazon-delivery-service-partner-investment-safety-ai-tools)).

## Awards

| Year | Award | Work recognized |
| --- | --- | --- |
| 2025 | Innovation Award, Amazon Last Mile Geospatial All Hands | GeoAI multi-agent framework on AWS Bedrock AgentCore (22 production tools, 10 sub-agents) |
| 2025 | People's Choice Award, Amazon GenAI Hackathon | Agentic prototype for geospatial analysis, with Ravi Garg, Dennis Billagiri, and Shaishav Maisuria |
| 2024 | Special Award for Operational Excellence, Amazon Geospatial Hub Winter Hackathon | Oncall Whisperer, an LLM assistant for on-call incident triage |
| 2023 | 1st Place, Amazon GS Hub Hackathon | Understanding driver building entry and exit events from raw GNSS signals |
| 2019 | Best Overall Award, Amazon Last Mile HackDay | Grid-based map tile ingestion |

## Writing

- [Agentic AI's Next Frontier Is the Physical World. Trust Will Decide Who Wins.](https://aijourn.com/agentic-ais-next-frontier-is-the-physical-world-trust-will-decide-who-wins/) The AI Journal, Jul 2026.
- [The Agent Drafts, a Human Approves: Inside State of the Map US 2026](https://hackernoon.com/the-agent-drafts-a-human-approves-inside-state-of-the-map-us-2026). HackerNoon, 2026.
- [How Open Source Runs the Mapping World](https://hackernoon.com/how-open-source-runs-the-mapping-world). HackerNoon, Jun 2026.

## Community and service

- Overture Maps Foundation: participant in the Schema and Buildings task forces; led Amazon's delivery-maps migration onto Overture data, schema, and GERS identifiers.
- Reviewer interests: LLMs and agentic AI for geospatial tasks, scalable spatial pipelines, map conflation, intelligent transportation.
- Mentor to engineers and researchers in big data and applied AI, inside Amazon and on ADPList; 300+ technical interviews conducted.

## Toolbox

`Spark` `Apache Sedona` `DuckDB` `GeoParquet` `Planetiler` `PMTiles` `MapLibre GL` `OSRM` `PostGIS` `Overture Maps` `OpenStreetMap` `AWS Bedrock AgentCore` `Strands Agents` `PyTorch` `Scala` `Python` `Java` `AWS`

<div align="center">
<img src="./assets/speaking-sotm-us-2026.jpg" alt="Vishal Kumar speaking at State of the Map US 2026" width="88%">
<br><sub>Speaking at State of the Map US 2026, Madison, WI.</sub>
</div>

## Contact

Research collaboration, program committee work, or comparing notes on maps and large-scale spatial data: reach me at vishku@amazon.com or on [LinkedIn](https://www.linkedin.com/in/vishalnitt/).
