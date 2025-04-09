# 🌍 Flag Quiz App

A simple web-based flag quiz built with Node.js, Express.js, and PostgreSQL.

## 🚀 Description

This app displays a random flag and asks users to guess the correct country name. It uses a PostgreSQL database to store country names and flag emojis or URLs. Scores are tracked for each session, and questions are dynamically rendered with EJS.

## 📦 Technologies Used

- Node.js
- Express.js
- PostgreSQL (`pg`)
- EJS Templates
- Body-parser middleware

## 🗃️ Database Setup

Create a PostgreSQL database named `World`, and a table `flags` with the following structure:

```sql
CREATE TABLE flags (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100),
  flag TEXT
);
