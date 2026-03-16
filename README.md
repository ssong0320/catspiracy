# Catspiracy

Multiplayer cat murder mystery game. Create or join a game, collect clues via minigames, and catch the fish thief before time runs out.

## Database setup

Create a PostgreSQL database for the app. Either use an existing database or create one.

**Option A – SQL (psql or any client):**

```sql
CREATE DATABASE catspiracy;
```
---

## Backend setup

1. **Go to the backend folder:**

   ```bash
   cd backend
   ```

2. **Add a `.env` file** in the `backend` folder with:

   ```env
   DATABASE_URL="postgresql://USER:PASSWORD@localhost:5432/catspiracy"
   PORT=3001
   ```

   Replace `USER` and `PASSWORD` with your PostgreSQL username and password. Change the host/port if your Postgres runs elsewhere.

3. **Install dependencies and prepare the database:**

   ```bash
   npm install
   npx prisma generate
   npx prisma db push
   ```

4. **Start the backend:**

   ```bash
   npm run dev
   ```

   The server runs at `http://localhost:3001`.

---

## Frontend setup

In a **new terminal**:

1. **Go to the frontend folder:**

   ```bash
   cd frontend
   ```

2. **Install and run:**

   ```bash
   npm install
   npm run dev
   ```

3. Open the URL shown (e.g. `http://localhost:5173`).

