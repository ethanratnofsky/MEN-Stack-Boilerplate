# MEN Stack Boilerplate (Ethan's Version)

This repository contains a boilerplate for a REST API service that uses [MongoDB](https://www.mongodb.com/), [Mongoose](https://mongoosejs.com/), [Express.js](https://expressjs.com/), and [Node.js](https://nodejs.org/en/).

## Getting Started

### Prerequisites

-   [Node.js](https://nodejs.org/en/)
-   [MongoDB](https://www.mongodb.com/) project
-   [MongoDB URI](https://docs.mongodb.com/manual/reference/connection-string/)

### Installation

1. Clone this repository.
    ```bash
    git clone https://github.com/ethanratnofsky/MEN-Stack-Boilerplate.git
    ```
2. Navigate to the project directory.
    ```bash
    cd MEN-Stack-Boilerplate
    ```
3. Edit the following values in the `package.json` file.
    - `name`
        - This should be the desired name of your NPM package. It must be unique and lowercase.
    - `description`
        - This should be a short description of your project.
    - `keywords`
        - This should be a list of keywords that describe your project.
    - `author`
        - This should be your name.
    - `repository.url`
        - This should be the URL of your GitHub repository.
    - `bugs.url`
        - This should be the URL of your GitHub repository's issues page.
    - `homepage`
        - This should be the URL of your project's README file in your GitHub repository.
4. Create a `.env` file in the project directory.
    ```bash
    touch .env
    ```
5. Add the following environment variables to the `.env` file.
    ```
    MONGODB_URI=<your MongoDB URI>
    ```
6. Uncomment the following line in the `config/mongodb.js` file.
    ```javascript
    // mongoose.connect(process.env.MONGODB_URI);
    ```
7. Install the Node dependencies.
    ```bash
    npm install
    ```
8. Start the development server.
    ```bash
    npm start
    ```
9. Navigate to [http://localhost:3000](http://localhost:3000) in your browser.
10. Navigate to [http://localhost:3000/example](http://localhost:3000/example) to test the `example` router.

## File Structure

-   `app.js` - The entry point for the application.
-   `config/` - Configuration files.
    -   `mongodb.js` - Configuration for MongoDB.
-   `controllers/` - Controller files.
-   `models/` - Mongoose model files.
-   `routes/` - Route files.

## Development Notes

### Prettier Formatting

To format your code with the Prettier formatter, run the following command:

```bash
npm run format
```

Prettier formatting configurations are stored in the `.prettierrc` file.
