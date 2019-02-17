# Docker Scripts

Some basic docker scripts with demo applications inside for different languages that I might use from day to day

## Current Language

| Folder | Description |
|---|---|
| express-js | Simple hello world express JS application |

## Useful Docker Commands

| Command | Description |
|---|----|
| docker kill $(docker ps -q) | Kill all running containers |
| docker rm $(docker ps -a -q) | Delete all stopped containers |
| docker rmi $(docker images -q) | Delete all images |
