FROM golang:1.21-alpine AS builder

WORKDIR /app

COPY . /app

RUN CGO_ENABLED=0 go build -o server .

FROM scratch 

COPY --from=builder /app/server /server

EXPOSE 8080

CMD ["./server"]