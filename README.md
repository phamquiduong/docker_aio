# Docker all in one
- Make docker-compose for support developer

<br>

## Prepairing
### Copy file `.env.example` to `.env`
```bash
cp .env.example .env
```

<br>

## Postgresql + Pgadmin4
### Start docker
```bash
docker-compose --profile postgresql up --build -d
```

### Stop docker
```bash
docker-compose --profile postgresql down
```

### Note
- With Pgadmin4 with example enviroment config
  - Access: http://localhost:5050
  - Email: `admin@mail.com`
  - Password: `admin`
  - And now you can connect with PostgreSQL.
  - ⚠️ Important: The connect host of PostgreSQL is `postgresql` not `localhost`

- If you don't want to use Pgadmin4 you can use this command for start
  ```bash
  docker-compose up postgresql --build -d
  ```
