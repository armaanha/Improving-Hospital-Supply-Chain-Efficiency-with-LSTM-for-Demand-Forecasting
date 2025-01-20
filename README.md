# 🏥 Improving Hospital Supply Chain Efficiency with LSTM for Demand Forecasting  

Managing hospital supplies effectively is critical to ensuring high-quality patient care. This project leverages Machine Learning, specifically **Long Short-Term Memory (LSTM)** networks, to improve demand forecasting for essential hospital supplies, thereby enhancing inventory management and reducing stockouts.

---

## ✨ Project Overview  

Hospitals often face challenges like inaccurate demand forecasting and inventory inefficiencies, which can disrupt operations and patient care. This project addresses these challenges by:  

- 🔍 **Developing and implementing an LSTM model** to predict daily demand for critical supplies like gloves, surgical masks, and ventilators.  
- 📊 **Improving demand forecasting accuracy**, enabling better procurement planning and reducing stockouts.  
- 🚀 **Enhancing supply chain efficiency** through data-driven predictions and optimized inventory management.  

---

## 🔬 Methodology  

1. **Model Selection:**  
   - Utilized **LSTM**, a Recurrent Neural Network (RNN) architecture, for its ability to capture long-term dependencies in sequential data.  

2. **Dataset:**  
   - Sourced from Kaggle, containing 500 records with daily information about stock levels, usage, and procurement details for hospital supplies.  
   - Key Features: `Current Stock`, `Min Required`, `Max Capacity`, `Avg Usage Per Day`, and temporal data like `Day of Week` and `Month`.  

3. **Key Features of the Model:**  
   - Handles **sequential and temporal patterns** in supply usage.  
   - Includes **Dropout** and **Batch Normalization** for regularization.  
   - Optimized with the **Adam optimizer** and evaluated using **Root Mean Squared Error (RMSE)**.  

4. **Training Process:**  
   - Data split into training, validation, and testing sets using **TimeSeriesSplit** to preserve temporal order.  
   - Input sequences of 60 days used to predict the average usage for the next day.  

---

## 📊 Results  

The LSTM model achieved promising results:  

- **Demand Forecasting Accuracy:**  
  - Gloves: RMSE = **61.78**  
  - IV Drip: RMSE = **71.53**  
  - Surgical Masks: RMSE = **67.97**  
  - Ventilators: RMSE = **52.55**  

- **Impact:**  
  - Reduced stockouts for critical supplies.  
  - Enabled proactive inventory management, ensuring resource availability during peak demand.  

---

## 🌟 Why This Matters  

This project demonstrates the transformative potential of Machine Learning in healthcare supply chain management:  

- **Better Patient Care:** Ensures timely availability of supplies.  
- **Cost Efficiency:** Reduces overstocking and wastage.  
- **Operational Excellence:** Aligns inventory with dynamic demand patterns.  

---

## 📌 Future Work  

- Incorporating external factors like patient inflow and seasonal trends to improve accuracy.  
- Exploring additional forecasting models like **Prophet** for capturing temporal dependencies.  
- Validating the model on larger datasets and real-time data streams.  

---

## 💡 Technologies Used  

- **LSTM (Long Short-Term Memory)**: For sequential data forecasting.  
- **TensorFlow**: Framework for model development.  
- **TimeSeriesSplit**: For temporal data partitioning.  

---

## 🖼️ Visuals  

Below is a sample visualization comparing actual vs. predicted usage for critical supplies:  

<img width="890" alt="image" src="https://github.com/user-attachments/assets/4e6a7eed-21c2-4520-bfb8-be5c5bbcbe81" />

