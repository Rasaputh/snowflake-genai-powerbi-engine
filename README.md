Clinical Insight Engine: AI-Powered Healthcare Analytics

Snowflake + Generative AI (Cortex) + Power BI
This project demonstrates a full-stack data engineering pipeline designed to help healthcare providers manage large-scale patient data efficiently. By integrating Snowflake’s cloud data platform with Generative AI, I transformed over 312,000 raw medical notes into actionable clinical insights.

📖 The Project Story
1. Data Engineering in Snowflake
The foundation of this project is a dataset of 312,358 patient records.

Snowflake Storage: I loaded raw healthcare encounters into a centralized Snowflake warehouse to ensure data security and scalability.

Cortex AI (The Brain): Instead of manual review, I used Snowflake Cortex AI functions to process messy doctor notes.

Sentiment & Summarization: I engineered a pipeline that automatically generates patient summaries and calculates a "Distress Score" (1-10) for every encounter.

2. The Infrastructure Bridge (Azure)
To bridge the gap between my macOS development environment and Windows-native tools:

Azure Windows VM: I deployed a Windows Server Virtual Machine on Azure.

Power BI Connectivity: This allowed for the installation of the full Power BI Desktop suite to connect directly to the Snowflake cloud.

3. Real-Time Visualization (Power BI)
I built a live dashboard that acts as a "Command Center" for clinical staff.

DirectQuery: Used a live connection to Snowflake, ensuring that as soon as a doctor adds a note, the dashboard updates in real-time.

Clinical KPIs:

Total Patients Managed: Tracks the scale of the dataset (312k+ records).

High Distress Count: A "Warning Light" identifying patients with a score of 8 or higher.

Average Distress Score: A health check for the entire clinic population.

Interactive Slicers: Implemented searchable dropdowns and range sliders to allow doctors to filter by name, date, or severity.

🛠️ Technology Stack
Database: Snowflake (Data Warehouse)

AI/ML: Snowflake Cortex (LLM / Generative AI)

Cloud: Microsoft Azure (Windows VM)

BI Tool: Power BI Desktop (DirectQuery Mode)

Source Control: Git & GitHub via VS Code

💻 A Note on Development
For this project, I utilized a MacBook Air (M3) to manage the SQL and cloud infrastructure. While the dashboard was built via a Cloud VM, this workflow is optimized for a native Windows environment like the HP Envy x360 2-in-1, which provides the 16GB of RAM and local processing power necessary for low-latency BI development.
