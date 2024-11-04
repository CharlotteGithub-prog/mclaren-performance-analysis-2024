# mclaren-performance-analysis-2024
2024 Season McLaren Racing Performance Analysis for Focusing Car Development

---

## Overview

This repository contains an in-depth performance analysis of McLaren Racing’s 2024 Formula 1 season, focusing on areas to inform and enhance car development. The analysis is conducted using Python and Jupyter Notebooks (`.ipynb`), leveraging the `fastf1` library for telemetry, lap data, and event information.

The aim of this project is to analyse McLaren's performance data across races, identifying key insights in lap times, tire usage, aerodynamics, and vehicle dynamics to support data-driven improvements in car development and strategy.

---

## Table of Contents

- [Installation](#installation)
- [Data Sources](#data-sources)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Analysis Focus Areas](#analysis-focus-areas)
- [Contributing](#contributing)
- [License](#license)

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
├── data/                        # Folder for storing any supplementary data files
├── notebooks/                   # Jupyter notebooks for data analysis
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_lap_analysis.ipynb
│   ├── 03_telemetry_analysis.ipynb
│   └── ...
├── src/                         # Python scripts for additional data processing or utilities
├── requirements.txt             # Python dependencies
└── README.md                    # Project readme
