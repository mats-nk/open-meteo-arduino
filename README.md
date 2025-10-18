# open-meteo-arduino
Arduino library that fetch weather data from [Open meteo API](https://open-meteo.com/).

[Open meteo API](https://open-meteo.com/) is free and requires no registration. Only for non-commercial use and less than 10.000 daily API calls. 

## Requirements
- `#include <time.h>`
- `#include <TimeLib.h>`

### Optional
- `#include <NTPClient.h>`

### Hardware supported
 ESP32
- ESP8266 ??
- Others ??

### Settings

This is the default values for Open Meteo API

- Temperature Unit: Celsius
- Wind Speed Unit: km/h
- Precipitation Unit: Millimeter
- Timeformat: ISO8601 (e.g. 2025-08-27 YYYY-MM-DD)

## Functions
- ```getHourlyForecast(forecast, <Lat>, <Long>, epochTime);```
- ```getAirQualityForecast```

### ```getHourlyForecast```

For details read https://open-meteo.com/en/docs
- Temp
- Humidity
- Apparent_Temp
- Precipitation
- Weather_Code
- Pressure
- Cloud_Cover
- Visibility
- Wind_Speed
- Wind_Deg
- Wind_Gust
- Is_Day

- Wet_Bulb_Temperature_2m
- Cape
- Uv_Index
- Uv_Index_Clear_Sky

- Dew_Point
- Snow_Depth
- Lifted_Index
- Convective_Inhibition
- Precipitation_Amount
- Terrestrial_Radiation
- Diffuse_Radiation
- Direct_Radiation

### ```getAirQualityForecast```

For details read https://open-meteo.com/en/docs/air-quality-api

- European_Aqi
- Us_Aqi
- European_Aqi_Pm2_5
- European_Aqi_Pm10
- European_Aqi_Nitrogen_Dioxide
- European_Aqi_Ozone
- European_Aqi_Sulphur_Dioxide

- Pm2_5
- Pm10
- Carbon_Monoxide
- Carbon_Dioxide
- Nitrogen_Dioxide
- Sulphur_Dioxide
- Ozone
- Aerosol_Optical_Depth
- Dust
- Methane
- Formaldehyde
- Glyoxal
- Nitrogen_Monoxide
- Peroxyacyl_Nitrates

