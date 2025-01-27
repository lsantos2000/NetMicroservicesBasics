# Play.Inventory.Service

This is the Play.Inventory.Service, a microservice for managing inventory items in the Play application.

### Running the Service with Docker Compose

1. Ensure Docker is installed and running on your machine. You can download Docker from [here](https://www.docker.com/products/docker-desktop).

2. Navigate to the directory containing the `docker-compose.yml` file.

```sh
cd path/to/your/docker-compose-file
```

## Getting Started

### Prerequisites

- [.NET 5.0 SDK](https://dotnet.microsoft.com/download/dotnet/5.0)
- [MongoDB](https://www.mongodb.com/try/download/community)
- [RabbitMQ](https://www.rabbitmq.com/download.html)

### Installation

1. Clone the repository:

```sh
git clone https://github.com/yourusername/Play.Inventory.Service.git
cd Play.Inventory.Service
```

2. Install dependencies:

```sh
dotnet restore
```

3. Set up your environment variables:
   - `AllowedOrigin`: The allowed origin for CORS.
   - MongoDB connection string and database name.
   - RabbitMQ connection string.

### Running the Service with Docker Compose

1. Ensure Docker is installed and running on your machine. You can download Docker from [here](https://www.docker.com/products/docker-desktop).

2. Navigate to the directory containing the `docker-compose.yml` file.

```sh
cd source_code/Play.Infra/
```

3. Run the following command to build start the services using Docker Compose:

```sh
docker-compose up --build
```

4. The service should now be running. You can access the Swagger UI at:

http://localhost:5000/swagger/index.html

5. To stop the services, use:

```sh
docker-compose down
```

### Running the Service using your local machine

1. Start your locally installed MongoDB and RabbitMQ services.

2. Run the application:

```sh
dotnet dev-certs https --trust
dotnet run
```

### Usage

The service exposes the following endpoints:

- `GET /api/inventory`: Get all inventory items.
- `POST /api/inventory`: Create a new inventory item.
- `PUT /api/inventory/{id}`: Update an existing inventory item.
- `DELETE /api/inventory/{id}`: Delete an inventory item.

### Swagger

Swagger is used for API documentation. Once the service is running, you can access the Swagger UI.

### License

This project is licensed under the MIT License.

Note: Code based, and modified for demo purposes, on the source code of the YouTube video course "[ASP.NET Core Full Course For Beginners](https://www.youtube.com/watch?v=ByYyk8eMG6c)" by Julio Casal at https://dotnetacademy.io. I encourage you to visit this resource and thank the author for providing the original code.
