# brexit_exporter
Provides a way to visualize Brexit status in Prometheus

```
curl localhost:29319
# HELP britain_still_in_the_eu Is Britain still in the EU
# TYPE britain_still_in_the_eu gauge
britain_still_in_the_eu 1
```

## dependencies

Needs netcat and curl
Works best with whatever netcat version Debian has

## Docker image

https://cloud.docker.com/repository/docker/pawadski/brexit_exporter

## install and run

Use Docker, really   
-or-   
Put brexit_exporter somewhere and run it   

# bugs

No multiprocessing. If you are checking brexit status an unhealthy amount of times you may see lag.
