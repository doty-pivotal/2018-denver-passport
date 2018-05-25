# 2018-denver-passport
Use the 2018 Denver Passport data to practice some techniques

## Working Notes

The Denver Passport [website](https://www.thepassportprogram.com/denver).

They publish the list of locations as a [google map](https://www.google.com/maps/d/u/1/viewer?ll=39.72879130585982%2C-104.95363959999997&hl=en&hl=en&z=12&mid=1nEqlYikMTivGcPlNWJFw_VnczefoHUzQ)

And from there we can download the data in some kml format. 

## Links for ideas

+ https://github.com/dmishin/tsp-solver
+ https://ericphanson.com/posts/2016/the-traveling-salesman-and-10-lines-of-python/
+ http://pbpython.com/pandas-list-dict.html
+ https://simonwillison.net/2018/Apr/20/datasette-plugins/
+ https://simonwillison.net/2017/Dec/12/location-time-zone-api/
+ https://www.periscopedata.com/blog/postgres-recursive-cte


## Getting started

(leave this at the bottom so we can `cat README.md` for our quickstart).

```
docker run -it --rm -p 8888:8888 -v "$PWD":/home/jovyan/work jupyter/datascience-notebook start.sh jupyter lab
```
