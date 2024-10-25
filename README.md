# Ecommerce Monorepo

# Monorepo Overview

This monorepo contains multiple packages and services managed together using [Turborepo](https://turbo.build/).
Turborepo helps in orchestrating builds, tasks, and dependencies efficiently across multiple projects.

## Description

Demo ecommerce web app for demonstrating the knowledge of the MERN stack.

## Prerequisites

### A typical top-level directory layout

    .
    ├── apps                    # Contains the main applications within the monorepo.
        ├── client
            ├── src
            ├── package.json            # Libraries and Utilities used for client applications
        ├── server
            ├── src
            ├── package.json            # Libraries and Utilities used for server applications
    ├── turbo.json              # Turborepo configuration file that manages caching, parallelism, and task orchestration.
    ├── package.json            # Shared libraries and utilities used across multiple applications.
    └── README.md

### Install Node JS

Refer to https://nodejs.org/en/ to install nodejs

## Running the Application in local

Install all the npm packages. Go into the project folder and type the following command to install all npm packages (at
Parent level)

```bash
npm install
```

In order to run the application locally Type the following command

```bash
npm run dev
```

## Execute script for getting 50 products

```bash
ts-node .\apps\server\src\scripts\addProducts.ts
```

The client application runs on **localhost:3000**
The server application runs on **localhost:5000**

## Creating and running build

To create the build run the following command

```bash
npm run build
```
