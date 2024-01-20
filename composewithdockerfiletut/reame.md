git add . && git commit -m "added" && git push origin main

to run with docker file use this 
#  app:
    build:
      dockerfile: Dockerfile

# docker compose exec db mysql -u root -p       