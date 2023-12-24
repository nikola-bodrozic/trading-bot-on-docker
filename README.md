docker compose run --rm freqtrade download-data --config user_data/config.json --days 30 -t 5m
docker compose run --rm freqtrade backtesting --config user_data/config.json --strategy SampleStrategy