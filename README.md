# Trading bot in dry run mode

### Check Docker version and pull the image

```
docker compose version
```

Should be around 2.3

```
docker compose pull
```

### Load data

```
docker compose run --rm freqtrade download-data --config user_data/config.json --days 30 -t 5m
```

### Run simulation using downloaded data

```
docker compose run --rm freqtrade backtesting --config user_data/config.json --strategy SampleStrategy
```