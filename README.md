# AlumLink

## Table of Contents
- [Project Description](#project-description)
- [Features](#features)
- [Screenshots](#screenshots)
- [Development Setup](#development-setup)
- [Installation Instructions](#installation-instructions)


## Project Description

AlumLink is an open-source alumni directory solution designed for CUNY Law School graduates. It is a full-stack application built with React, Node.js, Express, and PostgreSQL. The app allows users to create a profile, look up other alumni, obtain geographical locations of where they're working, and connect with each other over a secure platform. Please note that the app is currently in development and is not yet ready for production use. It is being developed by CUNY Tech Prep fellows.

## Features

- User Registration and Profile Creation
- Alumni Directory Search
- Geographical Location of Alumni
- Secure Messaging Platform
- User Authentication

## Screenshots
<img width="1439" alt="Screenshot 2024-01-12 at 12 53 19 AM" src="https://github.com/jawadrada/AlumLink/assets/103535961/f23c2ab8-beb2-4ffa-aa01-4786014cea11">

## Development Setup

### Prerequisites

- [Node.js](https://nodejs.org/) (Versions 10-14 are recommended)
- [PostgreSQL](https://www.postgresql.org/) (Versions 10-14 should work)

### Create a PostgreSQL user and database
The project-starter template expects the following for local development:

### PostgreSQL User/Role
- name: `user`
- password: `pass`

### PostgreSQL Database
- name: `database_name`

### creating a local database with psql
Create a user in PostgreSQL named `username` with the password `password`:

- Command to create user: `createuser -P -s -e ctp_user`
- Command to create database: `createdb -h localhost -U username database_name`

## Installation instructions
`git clone "https://github.com/CUNYTechPrep/AlumLink.git"`

### Running the app locally
For local development, you will need two terminals open, one for the api-backend and another for the react-client.
Update the `config.json` file and `.env` in the api folder with the matching username, password, and database name

### To run the project 
cd into AlumLink and download the following dependencies in your terminal:

#### api-backend (terminal 1)
``` 
cd api
npm install
npm run migrate:up
npm run seed:up
npm run dev
```

#### react-client (terminal 2)
```
cd client
npm install
npm start
```

api-backend will launch at: `http://localhost:8080`  
react-client will launch at: `http://localhost:3000`  
