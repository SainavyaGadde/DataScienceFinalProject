# **Autonomous Household Energy Consumption Pattern Model Using Machine Learning Algorithms**

## **Introduction**
With the increasing emphasis on energy efficiency and environmental sustainability, managing household energy consumption has become a critical focus area. Rising energy costs and growing environmental concerns underscore the importance of optimizing energy use in smart homes. 

This project aims to address this challenge by leveraging machine learning algorithms to develop an **Autonomous Household Energy Consumption Pattern Model**. By analyzing historical energy consumption data, the model will predict future usage patterns, enabling homeowners to make informed decisions about appliance use. This initiative not only promotes cost savings but also supports sustainability efforts, paving the way for more energy-efficient smart homes.

---

## **Project Objectives**
This project is guided by the following objectives:
1. **Analyze** the effectiveness of machine learning algorithms in predicting household energy consumption patterns.  
2. **Develop** an autonomous model using LSTM, GRU, and RNN algorithms to identify energy usage trends.  
3. **Train and Test** the model using the Kaggle dataset on household energy consumption.  
4. **Evaluate** the model's performance to identify the algorithm that provides the most accurate predictions.

---

## **Research Questions**
The project seeks to answer the following key questions:
1. How can machine learning algorithms be used to develop an autonomous model for predicting household energy consumption patterns?  
2. Which machine learning algorithm—LSTM, GRU, or RNN—provides the most accurate predictions for household energy consumption?

---

## **Dataset Overview**
The dataset used for this project is the **Household Power Consumption Dataset**, available on [Kaggle](https://www.kaggle.com/datasets/imtkaggleteam/household-power-consumption/data). Key details include:
- **Source**: Real-world household energy consumption data.  
- **Features**: Includes attributes such as `Global_active_power`, `Voltage`, and `Sub_metering` values that represent various aspects of energy usage.  
- **Timeframe**: Covers several years of data, providing a rich source for training machine learning models.  
- **Goal**: Utilize this data to predict future energy consumption patterns.

### **Data Information Observations**

The dataset contains information on household energy consumption, with a total of **1,048,575 records** and **9 columns**. Below are the key observations based on the dataset overview and summary statistics:

#### **General Information**
- **Total Rows**: 1,048,575
- **Total Columns**: 9
- **Memory Usage**: Approximately 72.0 MB
- **Column Types**:
  - **Numerical**: 7 columns (`float64`)
  - **Categorical (Object)**: 2 columns (`Date`, `Time`)

The table below summarizes the attributes information available in the dataset

| **Attribute**        | **Description**                                                                                                                       | **Type**            |
|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------|---------------------|
| `Date`               | Date in format `dd/mm/yyyy`.                                                                                                         | String / Date       |
| `time`               | Time in format `hh:mm:ss`.                                                                                                           | String / Time       |
| `globalactivepower`  | Household global minute-averaged active power (in kilowatt).                                                                         | Numerical (float)   |
| `globalreactivepower`| Household global minute-averaged reactive power (in kilowatt).                                                                       | Numerical (float)   |
| `voltage`            | Minute-averaged voltage (in volt).                                                                                                   | Numerical (float)   |
| `global_intensity`   | Household global minute-averaged current intensity (in ampere).                                                                      | Numerical (float)   |
| `submetering1`       | Energy sub-metering No. 1 (in watt-hour of active energy). Corresponds to the **kitchen**, mainly a dishwasher, oven, and microwave. | Numerical (float)   |
| `submetering2`       | Energy sub-metering No. 2 (in watt-hour of active energy). Corresponds to the **laundry room**, e.g., washing machine, fridge, light. | Numerical (float)   |
| `submetering3`       | Energy sub-metering No. 3 (in watt-hour of active energy). Corresponds to **electric water-heater** and **air-conditioner**.         | Numerical (float)   |

#### **Missing Data**
- Approximately **0.3881%** of the rows in the numerical columns have missing values.
- The columns affected by missing values include:
  - `Global_active_power`
  - `Global_reactive_power`
  - `Voltage`
  - `Global_intensity`
  - `Sub_metering_1`
  - `Sub_metering_2`
  - `Sub_metering_3`

#### **Summary Statistics of Numerical Columns**

1. **Energy Consumption Distribution**:
   - The average household global active power (`Global_active_power`) is **1.108 kW**, with a maximum value of **10.67 kW**.
   - Reactive power (`Global_reactive_power`) is relatively low, averaging **0.118 kW**.
2. **Voltage Stability**:
   - Voltage values are relatively stable, with an average of **239.96 volts** and a standard deviation of **3.285 volts**.
3. **Energy Intensity**:
   - Household global intensity (`Global_intensity`) has a wide range, from **0.2 amperes** to a peak of **46.4 amperes**.
4. **Sub-metering Insights**:
   - Sub-metering values for different areas (kitchen, laundry room, and water heater/air-conditioner) indicate variations in energy usage across household zones, with sub-metering 3 having the highest average consumption (**5.934 watt-hour**).


The dataset provides a rich set of features for analyzing and predicting household energy consumption patterns. Addressing missing data and normalizing numerical features will be essential steps in the preprocessing phase to ensure model accuracy and reliability.


---

## **Models and Approach**
To achieve the project goals, the following machine learning models will be implemented:
1. **Recurrent Neural Network (RNN)**:  
   A foundational sequential model that learns time-dependent patterns.  

2. **Long Short-Term Memory (LSTM)**:  
   A powerful model capable of capturing long-term dependencies in time-series data using advanced gating mechanisms.

3. **Gated Recurrent Unit (GRU)**:  
   A simplified alternative to LSTM, known for its computational efficiency and ability to handle sequential data effectively.

The models will be trained and tested on the dataset under consistent hyperparameter configurations to ensure a fair comparison.

---

## **Workflow Overview**
1. **Data Preprocessing**:  
   Clean and preprocess the dataset, handling missing values and normalizing features.  

2. **Feature Engineering**:  
   Extract relevant time-series features, such as lag values and rolling statistics, to enhance model performance.  

3. **Model Development**:  
   Implement RNN, LSTM, and GRU architectures tailored for time-series forecasting.  

4. **Training and Evaluation**:  
   Train each model using predefined hyperparameters and evaluate their accuracy in predicting energy usage patterns.

5. **Comparison and Analysis**:  
   Compare the models to determine the most suitable algorithm for household energy consumption forecasting.

---
## **Final Results**
![image](https://github.com/user-attachments/assets/224b18be-bfa4-4ee6-b00a-3762549bbc5f)


## **Significance of the Project**
This project not only contributes to the field of smart home technologies but also provides a framework for building energy-efficient solutions. By integrating IoT-based systems with machine learning models, homeowners can monitor and optimize their energy usage effectively, reducing costs and supporting a sustainable future.
