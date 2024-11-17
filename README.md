# Solar Electricity Analysis and Battery Storage Optimization

## Project Overview
This project involves analyzing solar electricity generation, electricity usage, and battery usage data to understand the potential benefits of using a battery system to store excess solar electricity. The project utilizes the Python programming language along with popular data science libraries such as `pandas` for data manipulation, `numpy` for numerical operations, `matplotlib` for data visualization, and `datetime` for handling time-related data.

## Project Steps

### Step (i): Data Visualization and Checks
In this step, the project begins by loading the provided data from an Excel file (`Junior Data Analyst_Data.xlsx`) into a pandas DataFrame. The data contains information about solar electricity generation, electricity usage, and other relevant parameters. The goal of this step is to visualize and compare the average solar electricity generation and electricity usage for each hour of the day.

### Step (ii): Calculating Electricity Bought
This step calculates the electricity that needs to be bought from the provider by subtracting the solar electricity generation from the electricity usage. The `numpy` library is used to efficiently perform element-wise subtraction, ensuring that the result is non-negative (i.e., the electricity bought cannot be negative).

### Step (iii): Calculating Excess Solar Generation
In this step, the project calculates the excess solar electricity generated by subtracting electricity usage from solar electricity generation. Again, `numpy` is used to perform element-wise subtraction while ensuring the result is non-negative (i.e., excess solar electricity is not negative).

### Step (iv): Modeling Battery Charge Level
This step models the cumulative battery charge level over time. The project assumes a maximum battery capacity of 12.5 kWh. The battery charge level is updated iteratively, considering the excess solar electricity generated and limiting the charge to the maximum capacity of the battery.

### Step (v): Calculating Electricity Bought with Battery
In this step, the project calculates the electricity that would need to be bought from the provider when using the battery to store excess solar electricity. This calculation subtracts the excess solar generation from the previously calculated electricity bought, assuming that stored battery energy is used to reduce the need for external electricity.

### Step (vi): Calculating Savings from Installing a Battery
This step calculates the potential savings from installing a battery by comparing the cost of electricity bought from the provider with and without the battery. The price of electricity is assumed to be $0.17 per kWh. The savings are quantified by computing the cost difference between the two scenarios.

### Step (vii): Data Aggregation and Visualization
The project aggregates the data on a monthly basis to provide a broader perspective. The aggregated values include total solar generation, electricity usage, electricity bought without a battery, and electricity bought with a battery. These aggregated values are visualized using a grouped bar plot, with each month represented on the x-axis and the respective values on the y-axis.

## How to Run the Project

### Prerequisites

Before running the project, ensure you have the following Python libraries installed:

- `pandas` - for data manipulation
- `numpy` - for numerical operations
- `matplotlib` - for data visualization


You can install these libraries using `pip`:


