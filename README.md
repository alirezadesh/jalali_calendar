# Jalali Calendar JSON Data

This repository provides detailed Jalali (Persian) calendar files in JSON format, covering each year with daily information. The data includes official holidays, events, and equivalent Gregorian dates, making it perfect for Persian date-based applications.

## Features

- **Comprehensive Daily Data**: Each day includes Persian and Gregorian dates, week information, and holiday markers.
- **Public Holidays**: Clearly marked official holidays.
- **Events and Occasions**: Lists national, global, and cultural events along with additional descriptions where relevant.

## File Naming Convention

Files are named based on the Jalali year, followed by `_data.json`, for easy access and reference:

```plaintext
1400_data.json
1401_data.json
1402_data.json
...
```

## JSON Structure

The JSON files contain information about each day in the Jalali calendar with the following structure:

```json
[
  {
    "date": "1400-01-01",
    "date_latin": "2021-03-21",
    "year_day": 1,
    "year_day_latin": 80,
    "month": {
      "name": "فروردین",
      "name_latin": "March"
    },
    "week": {
      "day": {
        "number": 2,
        "name": "یک‌شنبه",
        "name_latin": "Sunday"
      },
      "year": {
        "number": 1,
        "number_latin": 12
      }
    },
    "is_holiday": true,
    "events": [
      {
        "description": "جشن نوروز/جشن سال نو",
        "additional_description": "",
        "is_holiday": true,
        "is_religious": false
      },
      {
        "description": "روز جهانی شعر",
        "additional_description": "21 March",
        "is_holiday": false,
        "is_religious": false
      },
      {...},
      ...
    ]
  },
  {...},
  ...
]
```


### Key Fields

- **`date`**: The Jalali date in `YYYY-MM-DD` format.
- **`date_latin`**: The corresponding Gregorian date.
- **`year_day`**: The day of the year in Jalali.
- **`year_day_latin`**: The day of the year in Gregorian.
- **`month_name`** and **`month_name_latin`**: Jalali and Gregorian month names.
- **`week_day`** and **`week_day_name`**: Jalali day of the week and name.
- **`is_holiday`**: Indicates if the day is an official holiday.
- **`events`**: A list of events with `description`, `additional_description`, `is_holiday`, and `is_religious` markers.
