git add . && git commit -m "added" && git push origin main
21/01/2024 dawai eye drop
docker compose --help

<!-- to create and run a container -->
# docker compose up -d

# docker compose config

# docker compose exec web bash

<!-- docker compose remove container  -->
# docker compose down --volumes
# docker compose down

<!-- env file  -->
# redis:${TAG}"

<!--  -->
# docker compose ls

# docker compose --profile rediscache config

# docker compose --profile rediscache down --volumes

# docker compose --profile rediscache up -d

# depends on servoce name (eg rcache web db)

<!-- to run cusotm name file -->
# docker compose -f docker-compose.dev.yml up -d