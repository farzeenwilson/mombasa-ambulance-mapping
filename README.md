# Spatial Optimization of Emergency Medical Services in Mombasa, Kenya 🚑📍

## Overview
This project applies spatial data science to evaluate and optimize emergency medical response coverage in Mombasa, Kenya. By mapping the critical window of medical response, this analysis visualizes driving isochrones from major hospitals to identify geographic blind spots in the city's emergency infrastructure. 

The goal is to bridge the gap between supply chain logistics and spatial analytics, providing a data-driven foundation for better resource allocation and emergency service procurement.

## The Problem
In dense urban environments, traffic congestion and suboptimal ambulance placement can severely delay response times. Identifying areas that fall outside a standard 10-minute driving window from major medical hubs (such as Coast General and Aga Khan Hospital) is critical for improving operational efficiency and community health outcomes.

## Methodology
This analysis is built iteratively, focusing on spatial mathematics and API integration:
1. **Base Mapping:** Rendering interactive city infrastructure.
2. **Spatial Routing:** Calculating real-world 5-minute and 10-minute driving isochrones using the OpenRouteService API to account for actual street networks.
3. **Coverage Analysis:** Generating simulated emergency coordinates and utilizing spatial geometry to mathematically determine the percentage of incidents occurring outside optimal coverage zones.

## Tech Stack
* **Language:** Python
* **Environment:** Jupyter Notebook / Google Colab
* **Libraries:** `folium`, `requests`, `shapely`, `json`
* **APIs:** OpenRouteService (ORS)

## How to Run This Project
1. Clone this repository or open `mombasa_ambulance_mapping.ipynb` directly in Google Colab.
2. Obtain a free API key from [OpenRouteService](https://openrouteservice.org/).
3. Insert your API key into the designated variable within the notebook.
4. Run the cells sequentially to generate the interactive maps and calculate coverage statistics.

## Future Scope
* Integrating historical traffic data for dynamic, time-of-day routing.
* Optimizing the theoretical placement of new ambulance dispatch hubs based on identified spatial blind spots.
* Overlaying population density data to weight the simulated emergency coordinates for more accurate risk assessment.
