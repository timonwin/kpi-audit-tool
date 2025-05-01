# KPI Audit Tool

A powerful AI-powered application that identifies meaningful metrics and eliminates vanity KPIs from your dashboards, helping teams focus on what actually drives business outcomes.

**Live Demo:** [https://kpi-audit-tool.vercel.app/](https://kpi-audit-dashboard.vercel.app/)

## Overview

The KPI Audit Tool solves a common business problem: dashboards cluttered with metrics that don't drive decisions. As highlighted in the challenge description, "Your dashboard tracks 27 KPIs. Two matter. The rest? Noise."

This application helps organizations:
* Identify and eliminate redundant, misleading, and zero-impact metrics
* Focus on KPIs that actually inform business decisions
* Get AI-powered recommendations for the most valuable metrics
* Visualize metric usage patterns across departments

## Features

* **Comprehensive Dashboard**: View your entire metrics landscape at a glance
* **Metric Usage Analysis**: Visualize how metrics are used across departments
* **Redundancy Detection**: Automatically identify duplicated metrics across teams
* **Intelligent Scoring System**: Score metrics based on multiple factors including:
  * Usage in decision making
  * Visibility in dashboards
  * Executive requests
  * Recency of review
  * Business goal alignment
* **Recommended KPIs**: Get AI-powered suggestions for your most valuable metrics
* **Problematic Metrics Identification**: Flag metrics that should be reconsidered or eliminated
* **Complete KPI Inventory**: Access a searchable, sortable table of all metrics
* **Advanced Filtering**: Filter metrics by various criteria
* **Export Functionality**: Download your analysis results

## Screenshots

### KPI Audit Dashboard
*Main dashboard showing metric statistics and usage patterns across departments*

### Recommended KPIs
*AI-powered recommendations showing the top 3 most impactful KPIs with score breakdowns*

### Problematic Metrics
*Organized view of redundant, misleading, and zero-impact metrics that should be reconsidered*

### Complete KPI Inventory
*Comprehensive view of all KPIs with detailed analysis and filtering options*

### Score Breakdown
*Detailed explanation of how metric scores are calculated with positive and negative factors*

## Scoring System

The KPI Audit Tool uses a comprehensive scoring system to evaluate each metric:

### Positive Factors
* **Used in Decision Making**: +30 points
* **Tied to Business Goals**: +25 points (based on goal/outcome keywords in interpretation notes)
* **Visible in Dashboards**: +15 points
* **Executive Requested**: +10 points
* **Recently Reviewed**: Up to +15 points based on recency
* **Recently Used for Decisions**: Up to +15 points based on recency

### Negative Factors
* **Misleading Metrics**: -25 points
* **Zero-Impact Metrics**: -20 points
* **Redundant Metrics**: -15 points (appears in multiple departments)

The final score is calculated by adding all positive factors and subtracting negative factors, then clamping the result between 0 and 100.

## Usage

### Loading Data
* Click "Load CSV Data" to upload your own CSV file
* The application supports analyzing CSV files with the following columns:
  * Department
  * Metric_Name
  * Visible_in_Dashboard
  * Used_in_Decision_Making
  * Executive_Requested
  * Last_Reviewed
  * Metric_Last_Used_For_Decision
  * Interpretation_Notes

### Analyzing Metrics
1. View the main dashboard for an overview of all metrics
2. Filter by department using the dropdown menu
3. Use "Advanced Filters" to refine your view
4. Explore different tabs to identify problematic metrics
5. Check the "Recommended KPIs" section for highest-scoring metrics
6. Export your analysis results with the "Export" button

## Installation

1. Clone the repository:
```
git clone https://github.com/yourusername/kpi-audit-tool.git
```

2. Navigate to the project directory:
```
cd kpi-audit-tool
```

3. Install dependencies:
```
npm install
```

4. Run the development server:
```
npm run dev
```

5. Open your browser and visit `http://localhost:3000`

## Technologies Used
* Next.js
* React
* Tailwind CSS
* Chart.js / Recharts

## Future Enhancements
* User Authentication: Multi-user support with role-based permissions
* Saved Reports: Save and share analysis results
* Historical Tracking: Monitor KPI performance over time
* Custom Scoring Rules: Define your own evaluation criteria
* BI Tool Integration: Connect with Power BI, Tableau, or Looker
* Team Collaboration: Add commenting and discussion features
* Mobile Optimization: Enhance the experience for on-the-go analysis

## License
This project is licensed under the MIT License - see the LICENSE file for details.

---

Built with Next.js and Tailwind CSS
