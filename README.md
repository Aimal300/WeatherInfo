# WeatherInfo

from pprint import pprint

API_key = '1df50b3d31c959d9e82f4db33fbee2a7' ###You will need to make your own account at openweatherapp.org to generate a key###

city = input("Enter a city: ")

base_url = "http://api.openweathermap.org/data/2.5/weather?appid="+API_key+"&q="+city

weather_data = requests.get(base_url).json()

pprint(weather_data)

