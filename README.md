# PostgreSQL Database Service with Docker and Docker-Compose

This repository provides a ready-to-use setup for deploying a PostgreSQL database service using Docker and Docker-Compose. It’s ideal for developers and teams who want to quickly and easily set up a database environment without hassle.

## 🚀 Features

- **Simplified Setup**: Includes a `compose.yml` file to define and run a PostgreSQL container with just one command.
- **Data Persistence**: Database data is stored in a Docker volume to ensure it is not lost when the container is removed.
- **Customizable Configuration**: Adjust PostgreSQL settings through environment variables in the `compose.yml` file.

## 🛠️ Requirements

- [Docker](https://docs.docker.com/get-docker/) (v20.10 or higher)
- [Docker-Compose](https://docs.docker.com/compose/install/) (v1.29 or higher)

## 🔧 Installation and Usage

1. **Clone the repository:**

   ```bash
   git clone https://github.com/ldcmleo/Postgress-Boilerplate.git
   cd your-repository
   ```
2. **Run Docker-Compose:**
   ```bash
   docker compose up -d
   ```

3. Access the Database:

You can connect to the PostgreSQL database using the PostgreSQL client or any compatible tool using the parameters specified in the docker-compose.yml file.

## 📝 Configuration
You can modify PostgreSQL settings in the compose.yml file. Key variables you can adjust include:
- POSTGRES_USER: Database username
- POSTGRES_PASSWORD: User password
- POSTGRES_DB: Database name to create

## 🔄 Updates

To update the service, stop and remove the existing containers, then start new ones with:

```bash
docker-compose down
docker-compose up -d
```

## 🤝 Contributing

Contributions are welcome. If you encounter any issues or want to add new features, feel free to open an issue or submit a pull request.

## 📄 License

This project is licensed under the MIT License.
