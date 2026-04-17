# Trade Anomaly Detection via. Snowflake ML

<img width="85" alt="map-user" src="https://img.shields.io/badge/views-011-green"> <img width="125" alt="map-user" src="https://img.shields.io/badge/unique visits-009-green">

Anomaly detection on financial trade data using Snowflake ML. Specifically within Snowflake's machine learning capabilities this example registers data from a Snowflake table into the feature store, prepares training and test datasets from the feature store, trains two variants of a classification model - logging them as part of an experiment. The best model from the experiment is registered with Snowflake's model registry where observability and lineage are available.

## How to deploy / use the code sample(s)

This repository can deploy the example described above. Follow these steps to deploy this example

1. Sample Data Set Up

   This notebook uses sample data from the [Sample_Data_Financial_Services](https://github.com/sfc-gh-csharkey/Sample_Data_Financial_Services) repository. You do not need to deploy the entire sample data repository. However, you must have the [trades data](https://github.com/sfc-gh-csharkey/Sample_Data_Financial_Services/blob/main/Capital_Markets/04_trades.sql) deployed as a Snowflake table.

   To make this data available run the SQL script [HERE](https://github.com/sfc-gh-csharkey/Sample_Data_Financial_Services/blob/main/Capital_Markets/04_trades.sql). It will create the table and populate it with data all via. a SQL script.

    The deployment expects you to use a database named ```FSI_DEMO_DB``` with a schema ```CAPITAL_MARKETS```. You can create these or use your database / schema of choice.

2. Run notebook for ML

     Upload the [trade_anomaly_detection.ipynb](https://github.com/sfc-gh-csharkey/Snowflake_ML_Trade_Anomaly_Detection/blob/main/trade_anomaly_detection.ipynb) to a Snowflake workspace and run the notebook cell by cell. Each cell includes a description of its purpose.
