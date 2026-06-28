# BookPlatform

BookPlatform is a demo web application for organizing and tracking a personal reading journey. Users can explore a collection of books, open detailed book pages, create an account, log in, manage a personal bookshelf, save favourite books, and view a profile.

> **Note:** This is a demo project optimized for desktop use and is currently not fully responsive.

## Features

- User registration and login
- Book catalogue with individual detail pages
- Personal bookshelf for tracking books
- Favourite books collection
- User profile page
- Client-side navigation with Vue Router
- Demo user data stored in a local JSON file
- Cookie-based session handling

## Technologies

- Vue.js 3
- Vue Router 4
- JavaScript
- HTML5
- CSS3
- Axios
- js-cookie
- JSON Server-compatible local data

## Project Structure

```text
book-platform-app/
├── db/
│   └── db.json
├── public/
├── Seminarska/
│   ├── book1/
│   ├── book2/
│   ├── ...
│   ├── MyProfile.vue
│   ├── myFave.vue
│   └── myShelf.vue
├── src/
│   ├── assets/
│   ├── components/
│   │   ├── Home.vue
│   │   ├── Login.vue
│   │   ├── SignUp.vue
│   │   └── WelcomePage.vue
│   ├── App.vue
│   ├── main.js
│   └── routers.js
├── babel.config.js
├── package.json
└── README.md
```

## Main Pages

The application includes:

- Home page
- Welcome page
- Sign-up page
- Login page
- My Shelf
- My Favourites
- My Profile
- Individual pages for more than 20 books

Some of the included titles are:

- *1984*
- *To Kill a Mockingbird*
- *Don Quixote*
- *Moby-Dick*
- *The Great Gatsby*
- *The Lord of the Rings*
- *Pride and Prejudice*
- *Anna Karenina*
- *One Hundred Years of Solitude*
- *Jane Eyre*
- *Hamlet*
- *Beloved*
- *The Hunger Games*
- *Gone Girl*

## Getting Started

### Prerequisites

Install:

- Node.js
- npm

### Clone the Repository

```bash
git clone https://github.com/veronika-ilioska/book-platform-app.git
cd book-platform-app
```

### Install Dependencies

```bash
npm install
```

## Run the Demo Database

The repository contains demo data in `db/db.json`. To expose it as a local REST API, install and run JSON Server:

```bash
npm install -g json-server
json-server --watch db/db.json
```

By default, JSON Server runs at:

```text
http://localhost:3000
```

Keep this terminal running while using the application.

## Run the Application

Open another terminal and run:

```bash
npm run serve
```

The Vue development server will display the local URL in the terminal, usually:

```text
http://localhost:8080
```

## Production Build

```bash
npm run build
```

The optimized production files will be generated in the `dist/` directory.

## Linting

```bash
npm run lint
```

## Available Scripts

| Command | Description |
|---|---|
| `npm install` | Installs project dependencies |
| `npm run serve` | Starts the development server |
| `npm run build` | Creates a production build |
| `npm run lint` | Checks and fixes linting issues |

## Demo and Security Notice

This project uses a local JSON file as a mock database and is intended only for learning and demonstration purposes.

The authentication system is not production-ready. Real applications should never store plain-text passwords or commit real user credentials to a repository. Use password hashing, secure server-side authentication, environment variables, and a proper database before deploying a production version.

## Author

**Veronika Ilioska**

- GitHub: [veronika-ilioska](https://github.com/veronika-ilioska)

## License

This project is intended for educational and portfolio purposes.
