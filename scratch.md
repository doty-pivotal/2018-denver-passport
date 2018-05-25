
```
def geocode(address):
    # print(address)
    google_geocode_api_base = 'https://maps.googleapis.com/maps/api/geocode/json?address={}'
    address_url = google_geocode_api_base.format(urllib.parse.quote_plus(address))
    response = requests.get(address_url)
    resp_json_payload = response.json()
    # print(resp_json_payload['results'][0]['geometry']['location'])
    
    point = resp_json_payload['results'][0]['geometry']['location']
    latitude = point['lat']
    longitude = point['lng']
    time.sleep(1)
    return latitude, longitude
```