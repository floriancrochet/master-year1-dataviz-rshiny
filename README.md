# Interactive Visualization of the 2024 French Legislative Elections
*A pedagogical R Shiny app for exploring and understanding the French legislative elections.*

---

## 🎯 Overview
This project is an interactive R Shiny application designed to inform users about the French legislative elections of 2024 through interactive visualizations, tables, and textual explanations.  

Developed as part of an academic Shiny training project, it combines web interactivity with data analysis and visualization to improve understanding of electoral mechanisms and party programs.

**Objectives**
- Present the functioning and importance of legislative elections in France  
- Visualize electoral results by city and constituency  
- Provide summaries of political parties’ programs  
- Enable dynamic exploration of information via maps, tables, and modals  

---

## 🗄️ Data
- **Source:** Data sources for the 2024 French legislative elections (local and national datasets)
- **Data Availability:** Provided in `data/`

---

## ⚙️ Features
- Navigate interactively through multiple tabs (`navbarPage`).  
- Explore constituencies using integrated maps with `leaflet`.  
- Generate dynamic tables with `DT`, including row color coding by political party.  
- Display detailed party programs and downloadable PDF files via modal windows.  
- Render textual explanations and HTML content for contextual education.  
- Render interactive graphics with `ggiraph`.  

---

## 🧰 Tech Stack
- **Language:** R  
- **Data Manipulation:** dplyr, tidyr, stringi  
- **Visualization:** shiny, shinyjs, shinythemes, leaflet, DT, ggiraph

---

## 📦 Installation
```r
install.packages(c("shiny", "shinythemes", "shinyjs", "leaflet", "DT", "stringi", "dplyr", "tidyr", "ggiraph"))
```

---

## 💻 Usage Example

### Reproducing the Analysis / Execution Pipeline
*(Expected runtime: ~5 seconds on AMD Ryzen 7)*

```r
shiny::runApp("project.R")
```

---

## 📂 Project Structure

```text
master-year1-dataviz-rshiny/
├── data/                                               # Electoral datasets
│   ├── cities_coordinates.rds                          # Geolocation data
│   ├── election_results_candidates_by_constituency.rds # Main election dataset
│   ├── unmapped_constituencies_all_rounds.rds          # Mapping edge cases
│   └── unmapped_constituencies_first_round.rds         # First round edge cases
├── www/                                                # Static assets
│   ├── assets/                                         # UI assets
│   └── references/                                     # Policy documents (PDFs)
├── LICENSE                                             # MIT License
├── README.md                                           # Project documentation
├── project.R                                           # Main Shiny app file
├── readme_instructions.md                              # Prompt instructions
└── template.md                                         # Template layout
```

---

## 📈 Results

*(The application functions primarily as an interactive exploratory dashboard. No explicit predictive performance metrics or analytical conclusions were formulated in the current scope).*

---

## 📚 References
- *support_formation_rshiny.pdf* — Training material on R Shiny structure, UI/server logic, and reactivity  
- Posit Shiny Gallery — https://shiny.posit.co/r/gallery/  
- Official Shiny documentation — https://shiny.posit.co/  

---

## 📜 License
This project is released under the MIT License.  
© 2025 Juliette Grison and Florian Crochet

---

## 👤 Authors
**Juliette Grison**  
[GitHub Profile](https://github.com/juliette-grison)  

**Florian Crochet**  
[GitHub Profile](https://github.com/floriancrochet)

*Master 1 – Econometrics & Statistics, Applied Econometrics Track* 

---

## 🤝 Acknowledgments
This work was conducted as part of an academic project on interactive data applications using R Shiny, supervised by **Marie Machefer**.  
Based on training resources from *support_formation_rshiny.pdf*. Special thanks to the R and Shiny open-source communities.
