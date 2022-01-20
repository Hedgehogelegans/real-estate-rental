# Real estate rental scraper

## Overview

Real estate rental scraper that extract data such as type of property, rent, number of rooms, location. Data is then stored in a PostgreSQL database for further analysis.

### Docker Compose

```console
$ docker build --tag real-estate-rental https://github.com/Hedgehogelegans/real-estate-rental.git#main
$ docker run --name real-estate-rental -e DB_HOST=HOST -e DB_USER=USER -e DB_NAME=NAME -e DB_PASSWORD=PASSWORD -e DB_PORT=PORT --network="bridge"  -p 5900:5900 -d real-estate-rental
$ docker logs real-estate-rental
```
