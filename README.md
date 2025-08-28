## 📌 Project Overview  
This project demonstrates a **log analytics and alerting workflow** using simulated B2B IT company data.  
It is designed for:  
- **Client demos** – Showcase SplunkForce capabilities in sales meetings.  
- **Sales decks** – Visuals and KPIs for leadership presentations.  
- **Training** – A starter-kit for interns and new team members to learn data pipelines & dashboarding.  

The solution is **self-contained** (dummy data only, no external infra) and aligns with SplunkForce’s B2B vision.  

---

## 🎯 Project Objectives  
- Generate realistic **dummy log data** (10,000+ entries).  
- Process & clean logs → **structured CSV/JSON output**.  
- Build an **interactive Power BI dashboard** with KPIs and alerts.  
- Deliver a **professional documentation + visuals** pack.  

---

## 📂 Repository Structure  

├── scripts/           # Python scripts for data generation & preprocessing  
├── data/              # Raw + cleaned datasets (CSV, JSON)  
├── dashboard/         # Power BI .pbix file + exported visuals  
├── README.md          # Project documentation  
└── docs/              # PDF report with screenshots  



---

## ⚙️ Scope of Work  

1. **Dummy Log Data Generation**  
   - Python script generates synthetic logs for B2B IT companies.  
   - Fields include: timestamp, company, app, endpoint, status code, response time, log level, user ID.  

2. **Data Processing & Preprocessing**  
   - Parsing, cleaning..  
   - Final outputs: `b2b_logs.csv` and `b2b_logs.json`.  

3. **Analytics Dashboard (Power BI)**  
   Key insights provided:  
   - 📈 **Error Rate Trend** (time-series view of failure %).  
   - 🔝 **Top 5 Endpoints by Failures**.  
   - ⏱ **Response Time Distribution** (Fast/Moderate/Slow).  
   - 🏢 **Error Rate by Company & Application**.  
   - 🛑 **Error Codes Breakdown (200, 400, 500, etc.)**.  
   - ⚡ **Alert View: Highlight when error% > 5%**.  

4. **Documentation**  
   - Step-by-step README (this file).  
   - Screenshots of dashboards.  
   - Exported PDF report for Sales & Demo teams.  

---

## 📊 KPIs & Metrics  

The Power BI dashboard highlights the following KPIs:  

- **Total Requests** → Count of all log events  
- **Total Errors** → Logs with status codes ≥ 400  
- **Error Rate (%)** → `(Total Errors / Total Requests) * 100`  
- **Average Response Time (ms)** → Mean of all response times  
- **Slow Responses (%)** → Requests where `response_time_ms > 1500`  

---

## 🔧 Tech Stack  

- **Python (pandas, mimesis, faker)** → Data generation & preprocessing  
- **Power BI** → Analytics dashboard & KPIs    
- **GitHub** → Repository & collaboration  

---

## 📸 Dashboard   

![Dashboard Main](https://github.com/Malav1301/b2b-log-generator/blob/main/Dashboard/Screenshot%202025-08-28%20234629.png)
