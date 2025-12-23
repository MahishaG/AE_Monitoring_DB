# Adverse Event Monitoring Dashbaord

## 📌 Project Overview
This project delivers a fully automated Power BI dashboard built to monitor adverse events (AEs) across two large-scale clinical trials. By joining and comparing query records with AE and related clinical form data, the dashboard intelligently flags whether an event is serious or not — enabling quick insights and better decision-making for trial teams. While scheduling the refresh, the on-premise files in the shared folder gets automatically overwritten through PowerShell scripts taken care by upstream team.

## 🔍 Key Insights
1. 🔁 Automated Refresh: Scheduled refresh (daily) to ensure near real-time monitoring
2. 🔗 On-preise dataset: Data connected from shared folder and connected through gateway for scheduled refresh.
3. 🔍 Smart Join Logic: Integrated 12 Excel-based datasets (~30K+ rows) 
4. 🛠 Power Query Transformations: Data cleaning, structuring, and transformation handled entirely in Power Query
5. 📊 User-Focused Visuals: Dashboard includes dynamic tables and clean layouts tailored for clinical teams

## 🔗 Join Logic Overview
1. Query Report → joined with Adverse Event using Subject ID & AE ID
2. Query Report → joined with combined AE-related forms using Subject ID & Related AE ID
3. Final output shows Seriousness (Yes/No) from matching rows
4. If no match, “Not Applicable” is filled using Power Query coalesce() logic

## Dashboard
<img width="577" alt="Zues_powerbi" src="https://github.com/user-attachments/assets/e3a77701-3e04-4a69-aa83-90e1bf7cb0f1" />

## Thank you!!!
