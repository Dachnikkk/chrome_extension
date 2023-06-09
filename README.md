# chrome-extension
nest-react-extension

In this work, an implementation of an extension will be presented that will allow the user to enter the words that he wants to learn. The developed extension is an innovative tool for people who are looking to improve their language skills and achieve more in their careers and personal lives. It allows users to easily add new words to their vocabulary list and easily learn them in context. Thanks to automatic translation, users can quickly and accurately understand the meanings of words, which greatly speeds up the process of learning a language.

## Tech Stack

**Client:** React, Axios, React-Calendar

**REST API:** NestJS, TypeScript, Prisma, PostgreSQL, Yandex-Cloud API


## Run Locally

Clone the project

```bash
  git clone https://github.com/Dachnikkk/chrome_extension.git
```

Go to the REST API directory

```bash
  cd back-end-diary
```

Install dependencies

```bash
  npm install
```

Install tables to database (you need to install PostgreSQL)

```bash
  npx prisma db push
```

Start the REST API server

```bash
  npm run start:dev
```

Go to the react directory

```bash
  cd front-end-diary
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run start
```

## API Login Reference

#### login user

```http
  POST /api/auth/login
```

| Parameter | Type     | Description                                   |
| :-------- | :------- | :---------------------------------------------|
| `id`      | `integer`| **Required**.  Id of user to fetch            |
| `email`   | `string` | **Required**. User Email                      |
| `password`| `string` | **Required**. Password of user, argon2 hashed |
| `accessToken`| `string` | **Response**. Access JWT token |
| `refreshToken`| `string` |**Response**.  Refresh JWT token |


## Feedback

If you have any feedback, please reach out to me.
