# gomicro prototype

This is a go-micro prototype generated using WeDAA, you can find documentation and help at [WeDAA Docs](https://www.wedaa.tech/docs/introduction/what-is-wedaa/)

## Prerequisites

- go version >= 1.20

## Project Structure

```
├── config/ (configuration properties loader)
├── controllers/ (api controllers)
├── docker/ (contains docker compose files for external components based on architecture design)
├── resources/ (configuration properties)
├── Dockerfile (for packaging the application as docker image)
├── README.md (Project documentation)
├── comm.yo-rc.json (generator configuration file for communications)
├── go.mod
└── main.go
```

## Get Started

Install required dependencies: `go mod tidy`

Run the prototype locally: `go run .`

Open [http://localhost:8086/hello](http://localhost:8086/hello) to view it in your browser.

The page will reload when you make changes.

## Containerization

Build the docker image: `docker build -t gomicro:latest .`

Start the container: `docker run -d -p 8086:8086 gomicro:latest`
