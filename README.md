# Biostream-Multimodel-AI
#  BioStream Multimodal AI

An autonomous, data-stream parser engineered to translate raw laboratory screenshots, data logging parameters, and clinical metrics into structured, clinical-grade summaries instantly.

##  The Inspiration
In biological research labs, biotech firms, and academic classrooms, interpreting raw data from cell culture tracking logs represents a major operational bottleneck. Researchers constantly capture visual screenshots of logging streams, spreadsheets, and system metrics. Manually transcribing these values, checking morphology statuses, and writing health summaries introduces human error and slows down discovery timelines. We wanted to build an autonomous agent that takes these messy logs and screenshots and turns them into a standardized structural layout instantly.

##  What It Does
**BioStream Multimodal AI** acts as a secure, intelligent parsing bridge for automated cell culture monitoring. The application accepts direct user uploads of **data logs and visual dashboard screenshots**.

When a user feeds a screenshot log stream into the terminal—using our primary validation string:
> *"Analyze this lab image. Data log stream: cell_conf: 0.78, active_mitosis_count: 14, morphology_status: stable, stress_ind: null."*

The agent immediately activates its internal reasoning loop. It strips away formatting noise, identifies key cell parameters, evaluates proliferation rates, and dynamically outputs a deterministic, clinical-grade overview report detailing confluence density, active division nodes, and sample viability.

---

##  Technical Architecture Overview
*   **Visual AI Orchestrator:** Dify Cloud
*   **Language Model Brain:** gpt-oss-120b
*   **Inference Infrastructure:** Groq Cloud 
*   **Ingestion Layer:** Native visual file upload nodes designed to accept screenshot matrices (PNG/JPG) alongside text strings.

---

## Detailed Breakdown of Cell Parameters (Showcase Example)
To prove the system's accuracy, the agent evaluates the core metrics from our primary cell log sequence as follows:

*   **`cell_conf: 0.78` (Cell Confluence):** The agent automatically extracts this value to identify that 78% of the surface area is covered by cell clusters, representing an optimal distribution.
*   **`active_mitosis_count: 14` (Active Division):** The engine isolates this metric to confirm that 14 distinct nodes are actively undergoing cell division, signifying rapid reproduction.
*   **`morphology_status: stable` (Cellular Shape):** The agent reads this flag to verify that cell boundaries are physically intact and completely normal.
*   **`stress_ind: null` (Stress Indicators):** The parser reads the null value to verify that zero toxicity, environmental shock, or culture degradation issues are present.

---

##  How to Import and Test This Workflow
To run this workflow inside your own environment:
1. Create a free account on [Dify.ai](https://dify.ai).
2. Navigate to your Studio dashboard and click **Create from Blank** -> **Import DSL file**.
3. Upload the configuration pipeline file included in this repository.
4. Bind your custom Groq API key configuration to the LLM node.
5. Hit **Publish**, open the **Preview** chat web app, and paste the test sequence to watch it compile!

##  What's Next for BioStream Multimodal AI
Moving forward, we plan to directly expand our visual node pipelines by connecting the agent's markdown parser to open-source medical lookup engines (like PubMed) to let the AI agent autonomously verify and cite peer-reviewed scientific journals for every visual anomaly or cell parameter it isolates.
