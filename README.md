# README


## Golang installation

[Download and install](https://go.dev/doc/install)



## Execute the API

Located in the path <golang-scaffolding-minimal/golang-api> execute the following command.

    go run ./cmd/api/
    

## API Endpoints

The available API endpoints are outlined below.
<br >

<details><summary><code> Health GET /health   </code></summary>

## 
Health Endpoint (pingpong)

- Request

```
curl -XGET 'localhost:8081/health'
```

Success Response:

 - Status Code: 200

</summary></details>

-----------------------------------------------------------

## Scaffolding (Understood as Project structure)

Golang promotes a package-oriented architecture. While there are many recommendations on structuring projects in Golang, there is no set standard. It depends on the type of project. To date, no standard is known.
Go Modules are based on Golang's package-oriented architecture.
Modules can be organized into packages, making it easy to reuse code.

```
+-- golang-scaffolding-minimal
+-- golang-api
\-- cmd / api
    +-- handlers.go
    +-- main.go
    +-- routes.go
\-- database
    +-- connection.go
+-- go.mod
+-- go.sum
+-- webapp
\-- public
    +-- index.html
\-- src
    +-- main.js
+-- README.md
```

### Scaffolding description

| Folder/File   | Description |
| -------- | ---------- |
| golang-api | Monolith or microservice name. It's generally the module's name.      |
| cmd / api     | All files in the main package are located in this folder.     |
| handlers.go | Defines the application's HTTP routes and associates it with the corresponding handlers.      |
| routes.go | Contains the functions that handle the logic of each HTTP route to process requests.      |
| main.go | Main entry point for a Golang application. defines the main() function that is executed when the application starts.       |
| database | All database package files are located in this folder.       |
| connection.go | Contains the database connector.       |
| go.mod | Describes the Go module dependencies.    |
| go.sum | Verifies the dependencies integrity.       |
| webapp | It's illustrative, so that the developer can place the webapp.       |


> At this stage the database and webapp folder are illustratives.

