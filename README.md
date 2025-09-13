# Bangladesh-Weather-Dataset-1901---2023-
This README document provides detailed information about a dataset that combines temperature 🌡️ and rainfall 🌧️ data. The temperature data is sourced from NASA's POWER Project, and the rainfall data is obtained from the Humanitarian Data Exchange (HDX) website, specifically focusing on Bangladesh rainfall data.
import pandas as pd

from google.colab import files
uploaded = files.upload()

file_name = list(uploaded.keys())[0]

df = pd.read_csv(file_name)

print(df.to_string(index=False))
