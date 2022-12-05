FROM golang:1.18-alpine

WORKDIR /app
COPY go.mod /app
COPY go.sum /app
RUN go mod download
COPY main.go /app

EXPOSE 8080
CMD go run main.go