# MM Performance Testing 

## How to use
- deploy [grafana](https://grafana.com/) & [influxdb](https://github.com/influxdata/influxdb) --> `docker-compose up -d`

- setup [dashboard](http://localhost:3000/dashboards) using [plugin](https://grafana.com/grafana/dashboards/2587)

- run tests --> `docker-compose run -v $PWD/tests:/scripts k6 run /scripts/tmp.js`

- review results --> `http://localhost:3000/`