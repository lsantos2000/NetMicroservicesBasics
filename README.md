# NetMicroservicesBasics

This repository contains a collection of microservices built using .NET. The microservices are designed to work together to form a cohesive system.

## Project Structure

- **NetMicroservicesBasics.sln**: The main solution file that includes all the projects.
- **nuget_packages/**: Contains NuGet packages used by the projects.
  - `Play.Catalog.Contracts.1.0.0.nupkg`
  - `Play.Common.1.0.0.nupkg`
  - `Play.Common.1.0.1.nupkg`
  - `Play.Common.1.0.2.nupkg`
- **postman_collections/**: Contains Postman collections for testing the services.
  - `Play.Catalog.Service.postman_collection.json`
  - `Play.Inventory.Service.postman_collection.json`
- **source_code/**: Contains the source code for the various microservices and common libraries.
  - **omnisharp.json**: Configuration file for OmniSharp.
  - **Play.Catalog/**: Contains the Play.Catalog microservice.
    - `.vscode/`: VS Code specific settings.
    - `src/`: Source code for the Play.Catalog microservice.
  - **Play.Common/**: Contains common libraries used by the microservices.
    - `.vscode/`: VS Code specific settings.
    - `src/`: Source code for the common libraries.
  - **Play.Frontend/**: Contains the frontend application.
    - `.env`: Environment variables for the frontend.
    - `.gitignore`: Git ignore file.
    - `.vscode/`: VS Code specific settings.
    - `LICENSE`: License file.
    - `package.json`: NPM package configuration.
    - `public/`: Public assets for the frontend.
    - `README.md`: Readme file for the frontend.
    - `src/`: Source code for the frontend.
  - **Play.Infra/**: Contains infrastructure-related code and configurations.

## Getting Started

### Prerequisites

- [.NET 8.0](https://dotnet.microsoft.com/download/dotnet/8.0)
- [Node.js](https://nodejs.org/) (for the frontend)

### Building the Solution

To build the entire solution, open a terminal and navigate to the root directory of the repository. Then run:

```sh
dotnet build [NetMicroservicesBasics.sln]
```

### Running the Services

To run the services, navigate to the respective service directories and use the dotnet run command. For example, to run the Play.Inventory service:

```sh
cd ./Play.Inventory.Service
dotnet run
```

### Running the Frontend

To run the frontend application, navigate to the Play.Frontend directory and use the npm start command:

```sh
cd ./Play.Frontend
npm start
```

### Testing

Postman collections for testing the services are available in the postman_collections directory. Import these collections into Postman to test the APIs.

### License

This project is licensed under the MIT License.

Note: Code based, and modified for demo purposes, on the source code of the YouTube video course "[ASP.NET Core Full Course For Beginners](https://www.youtube.com/watch?v=ByYyk8eMG6c)" by Julio Casal at https://dotnetacademy.io. I encourage you to visit this resource and thank the author for providing the original code.
