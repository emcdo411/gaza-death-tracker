# 📊 Gaza Death Toll Dashboard

[![R](https://img.shields.io/badge/-R-276DC3?logo=r)](https://www.r-project.org/) [![Shiny](https://img.shields.io/badge/-Shiny-1abc9c?logo=rstudio)](https://shiny.posit.co/) [![Leaflet](https://img.shields.io/badge/-Leaflet-88cc88?logo=leaflet)](https://leafletjs.com/) [![Plotly](https://img.shields.io/badge/-Plotly-d62728)](https://plotly.com/) [![DT](https://img.shields.io/badge/-DT-33a02c)](https://rstudio.github.io/DT/) [![dplyr](https://img.shields.io/badge/-dplyr-1f77b4)](https://dplyr.tidyverse.org/) [![jsonlite](https://img.shields.io/badge/-jsonlite-e377c2)](https://cran.r-project.org/package=jsonlite) [![httr](https://img.shields.io/badge/-httr-17becf)](https://cran.r-project.org/package=httr) [![htmlwidgets](https://img.shields.io/badge/-htmlwidgets-9467bd)](https://www.htmlwidgets.org/)

## 🗂️ Table of Contents
- [📌 Summary](#summary)
- [🧩 Features](#features)
- [🛠️ Tech Stack](#tech-stack)
- [⚙️ Installation](#installation)
- [🚀 Usage](#usage)
- [💻 Code](#code)
- [📣 Why This Matters](#why-this-matters)
- [✅ Conclusion](#conclusion)

## 📌 Summary
The **Gaza Death Toll Dashboard** visualizes the humanitarian impact of the ongoing conflict in Gaza as of **June 2025**. The R Shiny app provides:

- A geospatial view of death tolls and hospital statuses across eight locations.
- A time-series breakdown of monthly deaths and cumulative tolls.
- Interactive visuals using a **military camouflage color palette** and Power BI-inspired dark theme.

📉 Over **62,614 deaths** reported (Al Jazeera, Jan 2025), and **55,000+ with hospital details** (Wikipedia, Jun 2025).

## 🧩 Features
### 🔍 Interactive Map
- Leaflet-based map focused on Gaza, Palestine, Israel.
- Clickable gray markers showing death counts, hospital status.
- Red marker for notable incident (young girl killed in Remal).
- Zoom level fixed for regional view.

### 📈 Line Graphs
- Dropdown to toggle between:
  - Cumulative Deaths
  - Monthly Death Rate
  - Deaths by Hospital Status
- Built with Plotly using camouflage shades for visual clarity.

### 📊 Bar Charts + Tables
- Bar chart of total deaths by location.
- Stacked bar: Deaths by hospital status.
- Exportable DT table with filters and full source annotations.

### 🎨 UX / Design
- Dark background (#252525), camouflage accents (#4a5a45 → #c4d17b), light text (#f0f0f0).
- Power BI-inspired layout: responsive containers with shadows and CSS-styled dropdowns.

## 🛠️ Tech Stack
- ![R](https://img.shields.io/badge/-R-276DC3?logo=r)
- ![Shiny](https://img.shields.io/badge/-Shiny-1abc9c?logo=rstudio)
- ![Leaflet](https://img.shields.io/badge/-Leaflet-88cc88?logo=leaflet)
- ![Plotly](https://img.shields.io/badge/-Plotly-d62728)
- ![DT](https://img.shields.io/badge/-DT-33a02c)
- ![dplyr](https://img.shields.io/badge/-dplyr-1f77b4)
- ![jsonlite](https://img.shields.io/badge/-jsonlite-e377c2)
- ![httr](https://img.shields.io/badge/-httr-17becf)
- ![htmlwidgets](https://img.shields.io/badge/-htmlwidgets-9467bd)

## ⚙️ Installation
```bash
# Clone the repository
$ git clone https://github.com/your-username/gaza-death-tracker.git
$ cd gaza-death-tracker
```

Install R and RStudio:
- [Install R](https://cran.r-project.org/)
- [Install RStudio](https://posit.co/download/rstudio-desktop/)

Install required packages in R:
```r
install.packages(c("shiny", "leaflet", "plotly", "dplyr", "DT", "httr", "jsonlite", "htmlwidgets"))
```

Run the app locally:
```r
shiny::runApp("app.R")
```

Optional: Deploy to [shinyapps.io](https://www.shinyapps.io/):
```r
install.packages("rsconnect")
rsconnect::deployApp(appDir = ".")
```

## 🚀 Usage
- Run the app.
- Use dropdowns to filter by location and graph type.
- Click on markers for popup insights.
- Hover over charts for tooltips.
- Download data table as CSV/Excel.

## 💻 Code
> 🔗 For full source code, see [`app.R`](./app.R)

```r
# Load dependencies
library(shiny)
library(leaflet)
library(plotly)
library(dplyr)
library(DT)
library(jsonlite)
library(httr)
library(htmlwidgets)

# ... (refer to app.R for full script)
```

## 📣 Why This Matters
> "We must bear witness to the human cost." — This dashboard helps humanize the conflict by visualizing deaths, hospital damage, and time-based escalation.

By presenting data in a modern, interactive format, this app:
- Fosters informed discussion.
- Supports humanitarian awareness.
- Documents regional destruction and health crises with clarity.

## ✅ Conclusion
The `gaza-death-tracker` app combines interactive GIS and statistical dashboards in a Power BI-style UI using the R ecosystem. It brings clarity to a humanitarian tragedy. Future enhancements may include:

- Real-time data from UN OCHA or Save the Children.
- Mobile-friendly layout with collapsible charts.
- New graph types for demographic breakdowns.

🙏 **Contribute** by forking the repo and submitting PRs.

---

© 2025 Maurice McDonald | Data Visualization for Justice | [GitHub](https://github.com/emcdo411) | [LinkedIn](https://www.linkedin.com/in/mauricemcdonald)

