
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


## Play with datasette
from https://conda.io/docs/user-guide/getting-started.html#before-you-start: 

```
#(not in the container - wanted to play with Datasette)
source $HOME/miniconda3/bin/activate
conda create --name passport
```

+ [Datasette](https://github.com/simonw/datasette)
+ [Building a location to time zone API with SpatiaLite, OpenStreetMap and Datasette](https://simonwillison.net/2017/Dec/12/location-time-zone-api/)
+ [Install Datasette Map Pluggin](https://pypi.org/project/datasette-cluster-map/)

