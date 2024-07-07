<p align="center">
  <img src="explode.png" alt="Explode Logo" width="25%" height="auto">
</p>

# <p align="center">Explode Music Streaming Platform</p>

## Setup

*Language/Framework:* Node.js with Express.js
*Database:* PostgreSQL
*Federation Protocol:* ActivityPub

## Dependencies

*express:* Web framework
*pg:* PostgreSQL client
*sequelize:* ORM for database interaction
*passport:* Authentication middleware
*passport-local:* Local strategy for federated login/signup
*stripe:* Stripe API for payment processing

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

Here's how it works:

### Federated Networking

Federated networking in Explode allows for a distributed architecture where multiple servers (instances) can communicate and share data seamlessly. Each instance of Explode acts as a node in a network, capable of independently managing users, content, and interactions.

### ActivityPub Integration

ActivityPub is a protocol that Explode uses to achieve federated social networking capabilities. It enables instances of Explode to exchange messages and notifications in a standardized way, promoting interoperability and user engagement across different servers.

### Key Features of Federated Networking and ActivityPub in Explode

  1. *Decentralization:* Users can join any instance of Explode and interact with users on other instances seamlessly. This decentralization ensures resilience and reduces dependency on a single server.
  
  2. *Interoperability:* ActivityPub allows users on different federated platforms (not just Explode instances) to follow, share, and interact with content from Explode. This opens up possibilities for broader audience reach and community building.

  3. *Privacy and Control:* Users retain control over their data and interactions. They can choose which instances to join and have the flexibility to migrate their accounts without losing their data, fostering trust and user empowerment.

  4. *Scalability:* Federated networking and ActivityPub support scalability by distributing the load across multiple servers. This architecture adapts well to growing user bases and varying traffic patterns without compromising performance.

## Implementation in Explode

  - *Backend:* The backend of Explode is designed with Node.js and PostgreSQL, incorporating ActivityPub protocols to handle federated interactions such as sharing playlists, following artists, and interacting with content from other federated instances.
  
  - *Frontend:* The frontend, built with Svelte and SvelteKit, integrates features that allow users to seamlessly navigate between different instances while maintaining a cohesive user experience.

By leveraging federated networking and ActivityPub, Explode not only enhances user engagement and content discoverability but also contributes to a more open and interconnected ecosystem of music streaming platforms.

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
