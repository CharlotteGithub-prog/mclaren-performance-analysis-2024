# mclaren-performance-analysis-2024
2024 Formula 1 season McLaren Racing performance analysis for focusing end of season car development.

**NB: To view analysis outputs view 'analysis' markdown file. Plots available in 'visualisations' directory.**

---

## Overview

This repository contains an in-depth performance analysis of McLaren Racing’s 2024 Formula 1 season, focusing on areas to inform and enhance car development. The analysis is conducted using Python and Jupyter Notebooks (`.ipynb`), leveraging the `fastf1` library for telemetry, lap data, and event information.

The aim of this project is to analyse McLaren's performance data across races, identifying key insights in lap times, tyre usage (future), track characteristics, aerodynamics (future), and vehicle dynamics to support data-driven improvements in car development and strategy.

---

## Table of Contents

- [mclaren-performance-analysis-2024](#mclaren-performance-analysis-2024)
  - [Overview](#overview)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
  - [Data Sources](#data-sources)
  - [Project Structure](#project-structure)

---

## Installation

To run this project locally, you will need Python 3.7+ and the necessary libraries as outlined below. It is recommended to set up a virtual environment for this project.

1. Clone the repository:

    ```bash
    git clone https://github.com/CharlotteGithub-prog/mclaren-performance-analysis-2024.git
    cd mclaren-performance-analysis-2024
    ```

2. Create a virtual environment:

    ```bash
    python -m venv venv
    source venv/bin/activate   # On Windows, use venv\Scripts\activate
    ```

3. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4. Jupyter Notebook setup (if not already installed):

    ```bash
    pip install notebook
    ```

---

## Data Sources

This project uses data provided by the `fastf1` Python library, which fetches real-time and historical Formula 1 data directly from Formula 1's API. The data includes telemetry, timing, weather, and session information, which are essential for detailed performance analysis.

---

## Project Structure

```plaintext
mclaren-performance-analysis-2024/
├── cache                                       # fastf1 data cache (set up locally)
├── venv/                                       # virtual project environment
│   └── ...
├── plots/                                      # Directory of individual analysis types
│   ├── plot_speed-heatmap_driver.ipynb         # Jupyter Notebook, season speeds by driver
│   ├── plot_speed-heatmap_team.ipynb           # Jupyter Notebook, season speeds by team
│   ├── plot_telemetry.ipynb                    # Jupyter Notebook, telemetry data by driver
│   ├── plot_track-characteristics_speed.ipynb  # Jupyter Notebook, season speeds by team
├── visualisations/                             
│   ├── AbuDhabi_TrackSpeed.png                 # Abu Dhabi Track Speed 
│   ├── Heatmap_McLaren_Ferrari_2024.png        # Heatmap comparing to Ferrari 2024 season
│   ├── Heatmap_McLaren_RedBull_2024.png        # Heatmap comparing to Red Bull 2024 season
│   ├── LasVegas_TrackSpeed.png                 # Las Vegas Track Speed 
│   ├── Qatar_TrackSpeed.png                    # Qatar Track Speed 
│   ├── Telem_LEC-NOR_Monza.png                 # Monza GP Leclerc vs Norris Telemetry
│   ├── Telem_PIA-VER_Brazil.png                # São Paulo Sprint Piastri vs Verstappen Telemetry
├── .gitignore                                  # Intentionally untracked files
├── 2024_season_overview.ipynb                  # Initial notebook
├── README.md                                   # Project readme
├── analysis.md                                 # FULL ANALYSIS FILE!
└── requirements.txt                            # Python dependencies 
