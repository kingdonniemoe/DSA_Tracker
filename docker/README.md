# Docker

This directory contains Docker Compose configuration for local development infrastructure.

Currently, it defines a Postgres database used by the backend API.

## Files

-`docker-compose.yml` - Docker Compose configuration
-`.env.example` - Template for required environment variables
-`.env` - Local environment file (not committed)

## Usage

Start the database:
`docker compose -f docker-compose.yml up -d`

Stop the databse (keep data):
`docker compose -f docker-compose.yml down`

Stop the database and delete all data:
`docker compose -f docker-compose.yml down -v`

## Notes
- Data persists across restarts unless `-v` flag is used
- This directory contains infrastucture only