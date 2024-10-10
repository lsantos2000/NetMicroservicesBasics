# Play Catalog Service

The Play Catalog Service is a microservice responsible for managing the catalog of items in the Play Economy project. It is built using .NET and follows a microservices architecture.

## Project Structure

### Directories

- **Play.Catalog.Service**: Contains the main service code for the catalog.
- **Play.Catalog.Contracts**: Contains the contracts used for communication between services.

## Getting Started

### Prerequisites

- [.NET SDK](https://dotnet.microsoft.com/download)

### Building the Project

To build the Play Catalog Service, navigate to the `Play.Catalog.Service` directory and run the following command:

```sh
dotnet build [Play.Catalog.Service](
```

### Running the Service

To run the Play Catalog Service, navigate to the Play.Catalog.Service directory and run:

```sh
dotnet run --project [Play.Catalog.Service]
```

### Testing

To run the tests for the Play Catalog Service, navigate to the test project directory and run:

```sh
dotnet test
```

### Contracts

The Play Catalog Service uses the following contracts defined in the Play.Catalog.Contracts project:

CatalogItemCreated
CatalogItemUpdated
CatalogItemDeleted

These contracts are used for communication between different services in the Play Economy project.

### Testing

Postman collections for testing the services are available in the postman_collections directory. Import these collections into Postman to test the APIs.

### License

This project is licensed under the MIT License.

Note: Code based, and modified for demo purposes, on the source code of the YouTube video course "[ASP.NET Core Full Course For Beginners](https://www.youtube.com/watch?v=ByYyk8eMG6c)" by Julio Casal at https://dotnetacademy.io. I encourage you to visit this resource and thank the author for providing the original code.
