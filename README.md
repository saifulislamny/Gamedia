# Gamedia

Social media site for gamers built using React, Node.js, Express.js, and PostgreSQL (PERN stack)

## Setup

1. Install [Node.js](https://nodejs.org/en/) (if you haven't already)
2. Install [Postgres](https://github.com/CUNYTechPrep/ctp2019/blob/master/guides/installing-postgresql.md) (if you haven't already)
3. Create a user in postgres named `ctp_user` with the password `ctp_pass`

```bash
createuser -P -s -e ctp_user
```

4. Create a postgres DB

```bash
createdb -h localhost -U ctp_user Gamedia
```

5. Clone this app

```bash
git clone https://github.com/saifulislamny/Gamedia
```

## Running the app

For local development you will need two terminals open, one for the API and another for the client.

1. Backend terminal

```bash
cp .env.example .env
npm install
npm run dev
```

2. Frontend terminal

```bash
cd client
npm install
npm start
```

3. Go to <http://localhost:8080> for backend
4. Go to <http://localhost:3000> for frontend

In production, only a single app is deployed. The react client will build into static files that will be served from the backend.
