# GameConnect Core

[![Quality Gate Status](http://146.190.150.93:9000/api/project_badges/measure?project=game-connect&metric=alert_status&token=sqb_444d47b12078e0727034ab6fab9967281f31939f)](http://146.190.150.93:9000/dashboard?id=game-connect)

This project is the core of the GameConnect platform, a social network for gamers. It provides a platform for gamers to connect, share, and play games together. The platform is designed to be user-friendly, secure, and scalable, making it suitable for both casual and competitive gamers. This project is a mono-repo that contains the core backend and frontend components of the GameConnect platform, using the `T3-Stack`.

This project is built on the [T3 Stack](https://create.t3.gg/) and is bootstrapped with `create-t3-app`. It integrates multiple cutting-edge technologies including Drizzle ORM for database interactions, Next.js for server-side rendering, NextAuth for authentication, and much more. This setup is designed to be scalable and efficient, making it suitable for both development and production environments.

## Technologies Used

- **[Next.js](https://nextjs.org)** - The React framework for production.
- **[NextAuth.js](https://next-auth.js.org)** - For secure authentication.
- **[Drizzle ORM](https://orm.drizzle.team)** - An ORM for managing database entities.
- **[Tailwind CSS](https://tailwindcss.com)** - For utility-first CSS.
- **[tRPC](https://trpc.io)** - End-to-end typesafe APIs made easy.
- **[Ansible](https://www.ansible.com/)** - For automating deployment and configuration.
- **[SonarQube](https://www.sonarqube.org/)** - For continuous inspection of code quality.
- **[PostgreSQL](https://www.postgresql.org/)** - As the underlying database system.

## Local Development Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Youngermaster/T3-Stack-Shadcn-UI.git
   cd T3-Stack-Shadcn-UI
   ```

2. **Install dependencies:**

   ```bash
   pnpm install
   ```

3. **Setup the environment:**
   Copy the `.env.example` file to `.env` and update the environment variables to match your setup:

   ```bash
   cp .env.example .env
   ```

4. **Start the local development database:**

   ```bash
   ./start-database.sh
   ```

5. **Run the development server:**

   ```bash
   pnpm dev
   ```

   Visit `http://localhost:3000` to view the application.

## Database Management

- **Migrate and push changes to the database:**

  ```bash
  pnpm db:push
  ```

- **Open Drizzle Studio to manage the database interactively:**

  ```bash
  pnpm db:studio
  ```

## Code Quality with SonarQube

Run SonarQube analysis to ensure high code quality:

```bash
./sonar_scanner.sh
```

Ensure SonarQube is running locally or adjust `SONARQUBE_URL` in your `.env` to point to your SonarQube server.

## Deployment

The application can be deployed using Docker. See the `docker-compose.yml` file for Docker configuration details. Use the following command to build and run the Docker environment:

```bash
docker-compose up --build
```

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Need Help?

If you have any questions or need help, please open an issue.
