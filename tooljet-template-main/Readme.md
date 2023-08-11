# ToolJet Boilerplate

## Local Setup

```
cp example.env .env
docker compose up -d

# Configure ToolJet. Can skip most of the options in the "survey"
```

# Setting Up External Database

While built-in database is available and enabled, this is used for isolation and easy migration of applications to production.

```
# Create new database
docker compose exec postgres psql -U postgres -w postgres -c 'create database test;'

# Add datasource named test with the following information
# Host: postgres
# User: postgres
# Password: postgres
# Database: test
```
