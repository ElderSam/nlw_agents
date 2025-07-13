# NLW Agents
typescript project

- Backend: API Rest with Gemini AI and database
- Frontend: React interact with API, getting question answer, create classes, upload audio files, etc.

## instructions

### docker
- run the container: ``docker compose up -d``
- ``docker-compose.yml`` defines services and depencencies.
- [pgvector](https://hub.docker.com/r/pgvector/pgvector/tags)

## drizzle ORM
- *drizzle-orm* is the orm for databases
- *drizzle-kit* is the CLI
- *drizzle-seed* helps you generate data to populate your database

1. Create migration:  
    ``npx drizzle-kit generate``

2. run migration:  
``npx drizzle-kit migrate``  

3. vizualize database (using the browser):  
``npx drizzle-kit studio``

OPTIONAL
Populate your database
``npm run db:seed``

## Testing routes
if you want, you can install the extension **REST Client** in **VSCode** and use the file ``client.http``