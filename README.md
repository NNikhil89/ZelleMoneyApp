- Clone the repo

```jsx
git clone https://github.com/NNikhil89/ZelleMoneyApp.git
```

- npm install
- Run postgres either locally or on the docker using DATABASE_URL

```jsx use the docker run command if connecting to Postgres using docker with the appropriate password
docker run  -e POSTGRES_PASSWORD=secretpassword -d -p 5432:5432 postgres
```

- Rename .env.example files to .env and give the valid Database url

- Navigate to `packages/db` and run the below commands to create database with seed values
    - npx prisma migrate dev
    - npx prisma db seed
- After DB creation run the app from command prompt by navigating to `apps/user-app` and then running the command `npm run dev`
- Try logging in using mobile number 1234567890 , password - tom
