FROM golang:1.21-alpine
WORKDIR /home/nonroot/route
COPY go.mod go.sum ./
RUN go mod download && go mod verify
COPY . .
CMD ["go", "run", "main.go"] # fix this asap
