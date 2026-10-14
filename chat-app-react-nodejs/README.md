# Snappy Chat

Snappy is a real-time chat application built with React, Express, MongoDB, and
Socket.IO. Users can create an account, choose an avatar, and exchange messages
with other users.


## Requirements

- [Node.js](https://nodejs.org/) and npm
- [MongoDB Community Server](https://www.mongodb.com/docs/manual/administration/install-community/) running locally or a MongoDB connection URL

## Getting started

1. Clone the repository and open the project directory.
2. Create environment files by copying each `.env.example` file to `.env`:
   - `server/.env.example` → `server/.env`
   - `public/.env.example` → `public/.env`
3. Configure the values in those files if needed. The backend example uses
   `mongodb://localhost:27017/chat` and port `5000`. The frontend example sets
   the local-storage key used for the current user. The frontend API connects
   to `http://localhost:5000`.
4. Install dependencies in both application folders:

   ```sh
   cd server
   npm install
   cd ../public
   npm install
   ```

5. Start MongoDB, then run the backend and frontend in separate terminals:

   ```sh
   cd server
   npm start
   ```

   ```sh
   cd public
   npm start
   ```

6. Open [http://localhost:3000](http://localhost:3000) in your browser.

Keep your `.env` files private; do not commit them.

## Available frontend scripts

Run these commands from `public/`:

| Command | Description |
| --- | --- |
| `npm start` | Start the React development server. |
| `npm test` | Run the tests in interactive watch mode. |
| `npm run build` | Create an optimized production build in `public/build/`. |

## Project structure

```text
public/   React client
server/   Express API, MongoDB models, and Socket.IO server
images/   README screenshots
```

## Acknowledgements

The project was inspired by this [chat application tutorial](https://www.youtube.com/watch?v=otaQKODEUFs).
