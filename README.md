# Aviation_Dataset
# ✈️ Airports Dataset

This dataset contains detailed information about airports worldwide. It can be used for geospatial mapping, flight network analysis, aviation analytics, and educational projects.

---

## 📁 Dataset Overview

| Column Name     | Description |
|-----------------|-------------|
| `id`            | Unique identifier for each airport |
| `name`          | Name of the airport |
| `city`          | City where the airport is located |
| `country`       | Country where the airport is located |
| `iata`          | IATA airport code (3-letter code) |
| `icao`          | ICAO airport code (4-letter code) |
| `latitude`      | Geographical latitude |
| `longitude`     | Geographical longitude |
| `altitude`      | Altitude of the airport (in feet) |
| `timezone`      | Timezone offset from UTC |
| `dst`           | Daylight saving time zone indicator |
| `tz_database`   | Timezone name as per TZ database |
| `type`          | Type of airport (e.g. `large_airport`, `small_airport`) |
| `source`        | Source of the data |

> **Note**: Column names may vary slightly depending on the version of the dataset.

---

## 🔍 Sample Use Cases

- Visualizing global airport distribution using maps
- Route planning or network modeling in air travel
- Identifying country-wise or city-wise airport density
- Dataset for machine learning and clustering tasks in the travel industry

---

## 📊 Dataset Info

- **Rows**: ~10,000+ (depending on source)
- **Columns**: 14
- **Format**: CSV
- **Encoding**: UTF-8

---

## 📦 How to Use

```python
import pandas as pd

# Load the dataset
df = pd.read_csv("airports.csv")

# Preview
df.head()

# Example: Filter airports in a specific country
df[df['country'] == 'India']
