
New York City DOT Real-Time Traffic Speed Application
=====================================================

This web application queries NYC traffic speed data and returns it in either JSON format or as a Mapbox map with color coded routes indicating speed ranges.

# Links

- [Python Flask](http://flask.pocoo.org/)

- [Explore Flask](http://exploreflask.com/en/latest/index.html)

- [Mapbox](https://www.mapbox.com/)

- [NYC Real-Time Data Feeds](http://www.nyc.gov/html/dot/html/about/datafeeds.shtml#realtime)

- [Traffic Sensors Metadata](http://a841-dotweb01.nyc.gov/datafeeds/TrafficSpeed/metadata_trafficspeeds.pdf)

- [NYC DOT real-time link speed query](http://207.251.86.229/nyc-links-cams/LinkSpeedQuery.txt)


# Installation
```
conda -V
conda update conda
conda info --envs
conda create --name nycdotspeed python=3
source activate nycdotspeed
conda install -c conda-forge flask-restful
conda install -c conda-forge requests
python app.py
```

# Usage

The following URLs can be used to access the NYC DOT real-time traffic speed data:

1. Mapbox map of New York City with color coded routes indicating real-time traffic speed:
```
http://127.0.0.1:5000/trafficspeeds
```
2. URL to return NYC DOT real-time link speed query as JSON:
```
http://127.0.0.1:5000/linkspeedquery
```
