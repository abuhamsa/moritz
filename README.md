## Moritz
Get instantly notified in Slack when a new offer that matches a search query gets published on Tutti.ch

### Usage
```
docker build -t moritz

docker run --rm \
  -e "SLACK_API_TOKEN=YOUR_API_TOKEN" \
  -e "SLACK_CHANNEL=moritz" \
  -v ~/.moritz:/usr/src/app/data \
  -it moritz:latest python --search="roomba"
```