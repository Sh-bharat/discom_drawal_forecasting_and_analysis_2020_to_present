# Discom Drawal Forecasting and Analysis (2020–Present)

This project involves extracting, consolidating, and forecasting hourly DISCOM drawal data from the UK SLDC portal, spanning from 2020 to the present. The workflow includes automated data scraping, integration with a MySQL database, and development of a time-series forecasting model using XGBoost. Model performance was evaluated on real data from January to April 2025.

---

## Summary of Work Completed

### Library Installation  
- **0_Installing_libraries.ipynb**  
  Installs all required Python packages necessary for data extraction, processing, modeling, and database operations.

### Data Extraction and Integration  
- **1_Creating_data.ipynb**  
  Automates scraping of DISCOM drawal data from the UK SLDC website across multiple years.  
- **2_merging_Files.ipynb**  
  Merges downloaded CSV files into a consolidated, clean dataset.  
- **3_Connecting_Mysql.ipynb**  
  Uploads the consolidated dataset into a locally hosted MySQL database.

### Forecast Modeling  
- **4_modeling.ipynb**  
  Develops and trains a forecasting model using XGBoost to predict hourly DISCOM drawal for May to July 2025. This notebook was executed in Google Colab for efficient model training and evaluation.

### Forecast Output  
- **XGBoost_Hourly_Forecast_May_July_2025.csv**  
  Contains the predicted hourly drawal values for the forecast horizon.

---

## Model Evaluation (January–April 2025)

The XGBoost forecasting model was evaluated on actual drawal data, yielding the following accuracy metrics:  
- RMSE: 42.36  
- MAE: 23.87  
- MAPE: 5.68%

![download](https://github.com/user-attachments/assets/a8c58edd-fa9d-4a5b-857c-147c270ef956)


---

## Technologies Used

- Python (Pandas, NumPy, XGBoost, SQLAlchemy)  
- Web Scraping (Requests, BeautifulSoup)  
- MySQL (Local instance)  
- Google Colab  
- Jupyter Notebooks

---

## Future Enhancements

- Automate regular data extraction and model retraining using scheduled workflows.  
- Explore advanced forecasting techniques such as LSTM or Transformer-based models.  
- Develop a deployment pipeline for real-time forecasting services.

---

## Acknowledgments

Thanks to GNA Energy for providing the project scope and valuable feedback during development.

---

## License

This project is intended for educational and research purposes. Contributions and forks are welcome with appropriate attribution.
