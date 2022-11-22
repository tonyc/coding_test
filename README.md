# Lightweight Coding Exercise

The goal of this coding exercise is to learn how you work and develop as a software engineer.

In this exercise, we will be making HTTP requests to parse JSON. You may use any gems you like,
and take any approach you like to solve the problem.

## Weather API

In this repository, you will find a file, `api.rb`, which has a URL. Build upon this file to make an HTTP request to the URL and parse the response body.

You may use any gems you like - feel free to add them to the Gemfile included in this repo.

1. Make an HTTP request to the URL. Display the latitude, longitude, and latest weather_code, temperature_2m, surface pressure, and windspeed.
2. Numeric weather codes aren't useful. Use this table of values to convert the numeric weather code to a description, and add it to the output

        0: Clear sky
        1, 2, 3: Mainly clear, partly cloudy, and overcast
        45, 48: Fog and depositing rime fog
        51, 53, 55: Drizzle: Light, moderate, and dense intensity
        56, 57: Freezing Drizzle: Light and dense intensity
        61, 63, 65: Rain: Slight, moderate and heavy intensity
        66, 67: Freezing Rain: Light and heavy intensity
        71, 73, 75: Snow fall: Slight, moderate, and heavy intensity
        77: Snow grains
        80, 81, 82: Rain showers: Slight, moderate, and violent
        85, 86: Snow showers slight and heavy
        95: Thunderstorm: Slight or moderate
        96, 99: Thunderstorm with slight and heavy hail

3. Add today's sunrise and sunset time to the output.
4. (optional?) A wind direction in degrees is also not always useful - write some code to convert the wind direction degrees returned into cardinal directions, i.e. N, NE, E, SE, S, SW, W, NW, and add it to the output.
