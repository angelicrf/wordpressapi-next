# WordPress-Next.js Integration

This project demonstrates the integration of a WordPress backend with a Next.js frontend, allowing users to authenticate, retrieve posts, and post new content directly from the Next.js application.

## Overview

This project demonstrates the integration of a WordPress backend with a Next.js frontend, allowing users to authenticate, retrieve posts, and post new content directly from the Next.js application.

## Features

Authentication: Users can authenticate using their WordPress credentials to access protected endpoints.
Retrieve Posts: Fetch and display WordPress posts in the Next.js application.
Create New Post: Users can submit new posts directly from the Next.js app to the connected WordPress site.

## Prerequisites

WordPress site with the JWT Authentication for WP REST API plugin installed and configured.
Node.js and npm installed on your machine.
Next.js application set up.

## Installation

Clone the repository:

```
git clone https://github.com/+++++.git

```

Install dependencies for both the WordPress and Next.js applications:

## Navigate to the WordPress plugin folder

```
cd wordpressapi-next/wp-plugin
npm install
```

## Navigate to the Next.js app folder

```
cd ../portfolio-next
npm install
```

Configure environment variables:

In the wordpress-nextjs-integration/wp-plugin folder, create a .env file with the following content:

```
WORDPRESS_API_URL=http://your-wordpress-site.com/wp-json
```

In the wordpress-nextjs-integration/nextjs-app folder, create a .env.local file with the following content:

```
WORDPRESS_API_URL=http://your-wordpress-site.com/wp-json
```

Replace http://your-wordpress-site.com with the URL of your WordPress site.

## Usage

## Instruction

iInstrunctions for building and running the project using Docker with a `docker-compose.yml` configuration file. Adjust the Docker commands and configuration to fit the specifics of your project if needed.

### Running with Docker

Build the Docker image:

```
docker-compose -f compose.yml build
```

Start the Docker containers:

```
docker-compose -f compose.yml up -d
```

Start the WordPress server:

# Navigate to the WordPress plugin folder

```
cd wordpress-nextjs-integration/wp-plugin
npm start
```

Start the Next.js application:

```
# Navigate to the Next.js app folder
cd ../portfolio-next
npm run dev
```

Open your browser and visit http://localhost:3000 to access the Next.js application.
