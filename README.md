# Stim — Game Catalog App

A Java desktop application for browsing and managing a personal game library, backed by MySQL. Users can register, log in, and manage their game collection — built as a university project.

## Features

- User registration and login
- Browse and search the game catalog
- Add, update, and remove games from your library
- MySQL-backed persistent storage

## Tech Stack

| Tool | Role |
|---|---|
| Java (Swing) | Desktop GUI |
| MySQL | Relational database |
| JDBC (MySQL Connector/J) | Java ↔ MySQL connectivity |

## Project Structure

```
src/
├── Connect.java    # JDBC connection helper
├── LoginForm.java  # Login screen
├── Register.java   # Registration screen
├── User.java       # User model
└── ...             # Additional screens
```

## Setup

1. Install Java 8+ and MySQL.
2. Import the database schema into MySQL (SQL file not included — create the `user` and `game` tables as referenced in the source).
3. In `src/Connect.java`, update `HOST`, `DATABASE_NAME`, and `USERNAME` to match your local MySQL configuration.
4. Add the MySQL JDBC driver to your classpath (not included — download from [dev.mysql.com](https://dev.mysql.com/downloads/connector/j/)).
5. Compile and run the main entry point.

## Skills demonstrated

- Java Swing GUI with multiple screens
- JDBC database connectivity
- User authentication flow
- Object-oriented Java design (model classes, separation of concerns)
