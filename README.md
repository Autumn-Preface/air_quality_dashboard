Project Title: Air Quality Visualization Dashboard (AQI Analyzer)

Overview:
The Air Quality Visualization Dashboard is a fully client-side, single-page web application for environmental data analysis. It allows users to upload multi-city air quality monitoring data in CSV format and instantly convert raw numbers into intuitive, interactive visualizations. Built with HTML, CSS, and JavaScript, it runs directly in the browser without any backend server or database, ensuring data privacy and simple deployment.

Key Features:

Multi-file Upload Management: Supports batch upload via click or drag-and-drop. Automatically parses CSV files, extracts city names from filenames, and merges them into a unified dataset. Users can view the uploaded file list and remove specific files dynamically.

Advanced Filtering Controls:

Date Range Picker: Filter data by custom start and end dates.

Dynamic City Selection: Auto-detects all available cities from uploaded data with "Select All / Deselect All" functionality.

Pollutant Metric Selector: Switch between different indicators (AQI, PM2.5, PM10, NO₂, SO₂, CO, O₃) for analysis.

Comprehensive Statistical Summary: Displays real-time key metrics including total records, number of cities, average AQI, maximum/minimum AQI, and the proportion of "Good" and "Excellent" air quality days.

Rich Visualization Gallery (7+ Chart Types):

Multi-city AQI Trend Line Chart – Compare AQI fluctuations across cities over time.
Calendar Heatmap – Visualize daily AQI intensity for a single city in a calendar grid.
Air Quality Grade Pie Chart – Show the proportional distribution of "Excellent," "Good," "Lightly Polluted," etc.
Pollutant Boxplot – Analyze the statistical distribution (median, quartiles, outliers) of six major pollutants.
Radar Chart – Compare average levels of multiple pollutants for a holistic city assessment.
Grouped Bar Chart – Contrast average pollutant concentrations across different cities.
Correlation Scatter Plot – Explore the relationship between two selected metrics (e.g., PM2.5 vs. AQI).
Interactive Dashboard Layout:

Responsive grid layout with adjustable chart cards.

Preset view modes: "Overview" (Trend + Heatmap + Pie) and "Deep Analysis" (Boxplot + Radar + Scatter).

Click-to-filter interactions (e.g., clicking a pie slice highlights corresponding data on the trend line).

One-click chart export as PNG images.

Theme Support: Toggle between Light and Dark modes.

Data Format:
The application expects CSV files with the following exact column headers (UTF-8 encoding):
日期, AQI指数, 质量等级, 当天AQI排名, PM2.5, PM10, NO2, SO2, CO, O3

File naming convention: CityName_YYYYMM.csv (e.g., Shanghai_202601.csv). The city name is automatically extracted from the file prefix.

Technology Stack:

Core: HTML5, CSS3 (Flexbox/Grid), Vanilla JavaScript (ES6+).

Charting: Apache ECharts 5 (via CDN).

CSV Parsing: Papa Parse (via CDN).

Deployment: GitHub Pages (fully static, no build tools required).

How to Use:

Clone or download the index.html file.

Open it directly in any modern web browser (Chrome, Edge, Firefox, Safari).

Upload your CSV files using the control panel on the left.

Interact with the filters and charts to explore your data.

Live Demo:
https://autumn-preface.github.io/air_quality_dashboard/

Repository Purpose:
This project serves as a practical tool for environmental researchers, data analysts, and citizen scientists to quickly visualize and interpret localized air quality trends without relying on internet connectivity or costly software.
