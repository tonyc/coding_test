# Lightweight Coding Exercise
## Weather API Client

The goal of this coding exercise is to learn how you work and develop as a software engineer.

In this exercise, we will be making HTTP requests to parse JSON. You may use any gems you like, and take any approach you like to solve the problem.

In this repository, you will find a file, `api.rb`, which has a URL. Build upon this file to make an HTTP request to the URL and parse the response body.

You may use any gems you like - feel free to add them to the Gemfile included in this repo.

1. Make an HTTP request to the URL. Display the latitude, longitude, and latest weather_code, temperature_2m, surface pressure, and windspeed.

2. Numeric weather codes aren't useful. Use this table of values to convert the numeric weather code to a description, and add it to the output.

        0: Clear sky
        1: Mainly clear
        2: Partly cloudy
        3: Overcast
        45: Fog
        48: Depositing rime fog
        51: Light drizzle
        53: Moderate drizzle
        55: Dense drizzle
        56: Light freezing drizzle
        57: Dense freezing drizzle
        61: Light rain
        63: Moderate rain
        65: Heavy rain
        66: Light freezing rain
        67: Heavy freezing rain
        71: Light snow
        73: Moderate snow
        75: Heavy snow
        77: Snow grains
        80: Light rain showers
        81: Moderate rain showers
        82: Heavy rain showers
        85: Light snow showers
        86: Heavy snow showers
        95: Thunderstorm
        96: Thunderstorm w/light hail
        99: Thunderstorm w/heavy hail

3. Add today's sunrise and sunset time to the output.

4. A wind direction in degrees is also not always useful - write some code to convert the current wind direction degrees returned into cardinal directions, i.e. N, NE, E, SE, S, SW, W, NW, and add it to the output.
   Hint: Consider a range of values around each "side" of the direction, e.g. NE is not just exactly 45 degrees.
