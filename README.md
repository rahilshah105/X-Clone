# X-Clone

**Interactive Twitter (X) clone built with Next.js, TypeScript, Prisma (MySQL), Tailwind CSS, and Docker.**

[![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)](https://nextjs.org)  
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org)  
[![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)](https://www.prisma.io)  
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)](https://www.mysql.com)  
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)  
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)](https://tailwindcss.com)  
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)

---

## Table of Contents

- [Features](#features)  
- [Tech Stack](#tech-stack)  
- [Getting Started](#getting-started)  
  - [Prerequisites](#prerequisites)  
  - [Installation](#installation)  
  - [Development](#development)  
  - [Building](#building)  
  - [Deployment](#deployment)  
- [Contributing](#contributing)  
- [License](#license)  
- [Contact](#contact)  

---

## Features

- CRUD operations for tweets, likes, reposts, follows—all persisted in MySQL via Prisma  
- User profiles and follower relationships managed server-side  
- Responsive UI with Tailwind CSS and dark mode toggle  
- Containerized services (app + database) with Docker & Docker Compose  

---

## Tech Stack

- **Next.js** (App Router & React 18)  
- **TypeScript** (static typing)  
- **Prisma** (ORM for MySQL)  
- **MySQL** (relational database)  
- **Docker & Docker Compose** (containerization)  
- **Tailwind CSS** (utility-first styling)  
- **ESLint** & **Prettier** (linting & formatting)  

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v16+  
- [Docker](https://www.docker.com/) & [Docker Compose](https://docs.docker.com/compose/)  
- Copy `.env.example` to `.env` and set `DATABASE_URL`  

### Installation

```bash
git clone https://github.com/rahilshah105/X-Clone.git
cd X-Clone
npm install
```

### Development

Bring up containers (app + MySQL) and run migrations:

```bash
docker-compose up --build -d
docker-compose exec app npx prisma migrate dev --name init
```

Then open [http://localhost:3000](http://localhost:3000) in your browser.

---

### Building

Create a production build inside the container:

```bash
docker-compose exec app npm run build
```

---

## Deployment

- Push to GitHub.  
- Deploy via a Docker-capable host (e.g., DigitalOcean, AWS ECS) using your Docker Compose setup.

---

## Contributing

1. Fork the repo  
2. Create a branch: `git checkout -b feature/YourFeature`  
3. Commit changes: `git commit -m "Add feature"`  
4. Push: `git push origin feature/YourFeature`  
5. Open a Pull Request

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Contact

🐙 **GitHub**: [https://github.com/rahilshah105/X-Clone](https://github.com/rahilshah105/X-Clone)  
✉️ **Email**: [superrahil10@gmail.com](mailto:superrahil10@gmail.com)
