# ContosoPizza

> An ASP .Net 8.0 RESTful API

## Create and explore a web API project

1. Make sure the version 8.0 SDK is installed
2. Create a new directory *ContosoPizza* for the project
3. In the directory, run this command: `dotnet new webapi -controllers -f net8.0`

This command creates the files for a basic web API project that uses controllers along with a C# project file named `ContosoPizza.csproj`

|Name|Description|
|----|-----------|
|Controllers/|Contains classes with public methods exposed as HTTP endpoints.|
|Program.cs|Configures services and the app's HTTP request pipeline, and contains the app's managed entry point.|
|ContosoPizza.csproj|Contains configuration metadata for the project.|
|ContosoPizza.http|Contains configuration to test REST APIs directly from Visual Studio Code.|

## Run and test the project

> Configure the certificates and launch settings to handle https connection.

Build the project with the following command: `dotnet run`. You should see the following output:  

```powershell
Building...
info: Microsoft.Hosting.Lifetime[14]
      Now listening on: https://localhost:7249
info: Microsoft.Hosting.Lifetime[14]
      Now listening on: http://localhost:5251
info: Microsoft.Hosting.Lifetime[0]
      Application started. Press Ctrl+C to shut down.
info: Microsoft.Hosting.Lifetime[0]
      Hosting environment: Development
info: Microsoft.Hosting.Lifetime[0]
      Content root path: F:\IT Projects\ADotNetLearningStory\Web Services\HttpRestApi\ContosoPizza
```

It is possible to see a JSON output at the URL: `https://localhost:7249/weatherforecast`, and a Swagger dashboard at the URL: `https://localhost:7249/swagger`.  
