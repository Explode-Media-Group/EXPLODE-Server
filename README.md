# Explode Music Streaming Platform

Explode is a federated music streaming platform that allows users to submit and stream music and podcasts. The platform includes an artist portal, user roles system, subscription system, and integrates with Stripe for payments. This repository includes both the frontend and backend components.

## Table of Contents

- [Features](#features)
- [Federated Infrastructure](#federated-infrastructure)
- [Frontend](#frontend)
- [Backend](#backend)
- [Installation Guide](#installation-guide)

## Features

- **Artist Portal**: Artists can submit music and podcasts with title, artist, album, description, image for album art, and tags.
- **User Roles System**: Manage different user roles such as admin, artist, and listener.
- **Subscription System**: Three subscription options with Stripe integration for payments.
- **Mobile Friendly**: Optimized for mobile devices.
- **Music Player**: Features play/pause button, share button, add to playlist button, and tip artist button using Stripe Connect API.

## Federated Infrastructure

Explode is built with a federated infrastructure using ActivityPub, enabling decentralized and distributed networking. This ensures scalability, resilience, and interoperability with other federated services.

## Frontend

The frontend of Explode is built using Svelte with SvelteKit for a fast and reactive user experience.

### Technologies

- **Svelte**: A modern, lightweight framework for building user interfaces.
- **SvelteKit**: A framework for building fast, server-rendered applications with Svelte.

## Backend

The backend is developed using Node.js and PostgreSQL to handle data storage, user authentication, and business logic.

### Technologies

- **Node.js**: JavaScript runtime for building scalable network applications.
- **PostgreSQL**: Advanced open-source relational database for storing and managing data.

## Installation Guide

Follow these steps to set up the Explode music streaming platform locally.

### Prerequisites

- Node.js (v14 or higher)
- PostgreSQL
- Git

### Clone the Repository

```
git clone https://github.com/yourusername/explode.git
cd explode
```

### Backend Setup
1. Navigate to the backend directory:

```
cd backend
```

2. Install backend dependencies:

```
npm install
```

3. Configure environment variables:
Create a .env file in the backend directory with the following variables.

```
DATABASE_URL=postgres://user:password@localhost:5432/explode
STRIPE_SECRET_KEY=your_stripe_secret_key
```

4. Run database migrations:

```
npx sequelize-cli db:migrate
```

5. Start the backend server:

```
npm start
```

### Frontend Setup

1. Navigate to the frontend directory:

```
cd frontend
```

2. Install frontend dependencies:

```
npm install
```

3. Configure environment variables:
Create a .env file in the frontend directory with the following variables.

```
VITE_API_URL=http://localhost:3000
```

4. Start the frontend server:

```
npm run dev
```

### Running the Application

Once both the backend and frontend servers are running, open your browser and navigate to http://localhost:3000 to access the Explode music streaming platform.

### Contributing

We welcome contributions from the community. Please read our Contributing Guidelines for more details.

### License

This project is licensed under the MIT License. See the LICENSE file for details.

### Contact

For any inquiries or support, please join [Explode's Discord Community](https://discord.gg/JqKeyyVXa2).
