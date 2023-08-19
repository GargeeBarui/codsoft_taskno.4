import requests
city = input("city name: ")

print(city)
print("display weather forecast of: ",city)
url = 'https://wttr.in/{}'.format(city)

req = requests.get(url)
print(req.text)
