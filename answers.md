# Advanced AI-Driven Urban Planning Tool

This tool allows you to:

- **Upload File**: Choose and upload a CSV or Excel file containing urban data (limit of 200MB per file).
- **Generate Synthetic Data**: Simulate urban scenarios or create mock data for various urban planning needs.
- **Data Sources**:
  - CSV
  - XLSX

The tool is designed to assist in analyzing urban data, simulating future scenarios, and improving decision-making with AI-driven insights.

# Data Preview

| time_period | area_id | lat           | lon            | population | traffic | green_space | crime_rate | avg_income | public_transport_access | air_quality_index | housing_density | commercial_area_percentage | healthcare_facilities | education_facilities | energy_consumption | water_usage | waste_generation | internet_connectivity | elderly_population_percentage |
|-------------|---------|---------------|----------------|------------|---------|-------------|------------|------------|--------------------------|-------------------|-----------------|----------------------------|----------------------|----------------------|-------------------|-------------|------------------|-----------------------|-----------------------------|
| 0           | 1       | 40.74908023769473 | -73.04928569   | 77820      | 5834    | 13.93       | 0.9997     | 117498     | 86.62                    | 120.22            | 710.99          | 5.93                       | 2                    | 24                   | 849.20            | 145.55     | 26.36            | 67.34                 | 12.61                       |
| 0           | 2       | 41.049512863264475 | -73.56805498   | 26658      | 2658    | 5.05        | 2.92       | 89150      | 45.61                    | 157.04            | 207.68          | 28.14                      | 3                    | 5                    | 646.79            | 126.74     | 15.85            | 97.96                 | 29.14                       |
| 0           | 3       | 41.61679469623292  | -73.69538623   | 69148      | 7141    | 20.84       | 4.40       | 78555      | 49.52                    | 6.88              | 910.23          | 16.65                      | 8                    | 4                    | 380.54            | 284.03     | 59.20            | 67.39                 | 29.24                       |
| 0           | 4       | 41.55026564672223  | -73.06050106   | 93093      | 1095    | 18.34       | 9.22       | 124663     | 57.04                    | 104.17            | 961.56          | 43.00                      | 13                   | 18                   | 585.72            | 314.04     | 96.87            | 84.28                 | 11.90                       |
| 0           | 5       | 40.592547011408165 | -73.83473306   | 49984      | 8106    | 13.28       | 3.95       | 32695      | 0.55                     | 163.09            | 709.79          | 37.81                      | 1                    | 27                   | 166.64            | 211.31     | 20.43            | 94.52                 | 20.58                       |

# Data Preview Explanation

The dataset contains various metrics for each area in an urban environment. Here's a breakdown of each column:

1. **time_period**: 
   - Represents the specific time period the data corresponds to. In this case, all entries are for time period 0.

2. **area_id**: 
   - An identifier for the geographical area or location within the urban environment (e.g., each area has a unique `area_id`).

3. **lat**: 
   - Latitude of the geographical area, representing its position on the Earth's surface (North-South).

4. **lon**: 
   - Longitude of the geographical area, representing its position on the Earth's surface (East-West).

5. **population**: 
   - The number of people living in the given area.

6. **traffic**: 
   - The level of traffic in the area, likely measured by the number of vehicles or congestion level.

7. **green_space**: 
   - The percentage of the area dedicated to green spaces, such as parks and recreational areas.

8. **crime_rate**: 
   - The level of crime in the area, possibly represented as the number of reported crimes per unit of population or area.

9. **avg_income**: 
   - The average income of residents in that area, likely indicating the socioeconomic status.

10. **public_transport_access**: 
   - The accessibility to public transportation services, possibly expressed as a percentage or an index of how well-connected the area is.

11. **air_quality_index**: 
   - A measure of the air quality, typically a scale that shows pollution levels and how safe the air is for residents.

12. **housing_density**: 
   - The number of housing units per unit of area, indicating how crowded or spacious the residential spaces are.

13. **commercial_area_percentage**: 
   - The percentage of the area used for commercial purposes (shops, businesses, etc.), reflecting urban development.

14. **healthcare_facilities**: 
   - The number of healthcare facilities (e.g., hospitals, clinics) available in the area.

15. **education_facilities**: 
   - The number of educational institutions (e.g., schools, universities) in the area.

16. **energy_consumption**: 
   - The amount of energy used in the area, which may reflect residential and commercial usage.

17. **water_usage**: 
   - The amount of water consumed in the area, likely representing both residential and industrial usage.

18. **waste_generation**: 
   - The amount of waste generated by the population in the area, possibly indicating the effectiveness of waste management and recycling systems.

19. **internet_connectivity**: 
   - The level of internet connectivity in the area, potentially reflecting broadband speeds or coverage.

20. **elderly_population_percentage**: 
   - The percentage of the population in the area that is elderly, which might be important for assessing healthcare and social services needs.

Each row represents a different area, with data points across multiple dimensions, useful for analyzing the quality of life, sustainability, and urban development in the areas.


# Advanced City Data Visualization Map

The **Advanced City Data Visualization** map is a tool designed to help visualize geographic and urban data in an interactive, spatial format. Here's a breakdown of its functions:

## Key Features:

### 1. **Geospatial Data Representation**:
   - The map visualizes data tied to specific geographical locations, such as areas, regions, or cities.
   - It displays data points like population density, traffic levels, green spaces, and other urban metrics based on latitude and longitude.

### 2. **Color-Coding & Heatmaps**:
   - The map may use color coding to represent different data values, such as:
     - **Green** for areas with high green space.
     - **Red** for areas with high traffic or crime rates.
     - **Blue** for areas with good air quality.
   - This helps users quickly identify trends and pinpoint areas needing attention.

### 3. **Interactive Exploration**:
   - Users can hover over or click on areas to view detailed information about the data for that location (e.g., population, traffic, or crime rate).
   - It allows zooming in/out to focus on specific areas or to see broader city/region perspectives.

### 4. **Dynamic Visualization**:
   - The map can show how various factors (like air quality, green space, or traffic) have changed over time, helping users analyze trends.

### 5. **Customization Options**:
   - Users may have the ability to choose which factors to display on the map, such as:
     - **Population density**
     - **Traffic congestion**
     - **Public transport accessibility**
     - **Crime rate**
     - **Energy consumption**
   - Customization allows for tailored visualizations based on user needs.

### 6. **Correlation with Urban Planning**:
   - The map helps visualize urban data in an intuitive way, making it easier to identify areas that need improvement or investment.
   - It is a valuable tool for urban planners to assess the impact of policies or create data-driven urban development strategies.

## Example Use:
For instance, if you want to understand how traffic congestion affects green space and population density, the map allows you to:
- Visualize traffic patterns across the city.
- See areas with more green space.
- Cross-reference population data with both traffic and green space data to make informed decisions about urban planning.

In summary, the **Advanced City Data Visualization Map** is a powerful tool for analyzing urban data and making data-driven decisions for city planning and development.


# Feature Importance Analysis and Urban Planning Simulation

## Feature Importance Analysis:
The **Feature Importance Analysis** tool helps you understand the relative significance of different factors affecting the selected **target variable**. In your case, **population** is chosen as the target variable.

### Available Target Variables:
The target variable can be selected from more than 10 available options such as:
- **Population**
- **Traffic**
- **Drainage**
- **Green Space**
- **Crime Rate**
- **Air Quality**
- **Commercial Area** and more.

These variables represent different aspects of urban life, and understanding how they relate to population (or any other chosen target) helps in making informed urban planning decisions.

### Performance Metrics:
- **Mean Squared Error (MSE)**: `72701.11`
  - This value indicates the average squared difference between predicted and actual values. Lower MSE values show better accuracy in predicting the target variable (population in this case).
  
- **R-squared Score**: `1.00`
  - An R-squared score of `1.00` means the model explains 100% of the variance in the target variable (population). This indicates a perfect fit between the model and data, suggesting that the selected features are highly predictive.

## Urban Planning Simulation:
Once the feature importance is understood, the **Urban Planning Simulation** allows you to create and simulate your own urban plan. This is done by adjusting various factors that influence city development.

### Focus Area for Proposals:
You can choose to focus on one or more areas for improvement, such as:
- **Traffic Optimization**: Improving traffic flow and reducing congestion.
  
### Key Variables for Custom Urban Plan Simulation:
You can adjust the following parameters to create a custom urban plan:
1. **Increase in Green Space (%)**: 
   - Set a percentage (0% to 100%) for how much green space you want to add. Green spaces can improve quality of life and contribute to environmental sustainability.
  
2. **Public Transport Expansion (%)**: 
   - Set a percentage (0% to 100%) for expanding public transport systems to reduce traffic congestion and improve accessibility.
  
3. **Renewable Energy Adoption (%)**: 
   - Set the adoption percentage (0% to 100%) for renewable energy sources like solar, wind, etc. This can help reduce carbon emissions and promote sustainability.
  
4. **Investment in Smart City Technologies (Million $)**: 
   - Set an investment amount (from $0 to $1,000 million) to improve technology infrastructure, such as smart grids, IoT devices, or AI-powered systems.
  
5. **Number of New Affordable Housing Units**: 
   - Set the number of new affordable housing units (e.g., 1,000 units) to address housing shortages and improve living standards.

### Simulation of Urban Plan:
- By adjusting these parameters, the tool simulates how your proposed changes will impact various aspects of urban life, such as:
  - Traffic flow
  - Green space availability
  - Energy consumption
  - Housing affordability
  - Public transport accessibility
  
This enables you to assess the effectiveness of your proposals before implementation, helping in creating more efficient and sustainable urban environments.

