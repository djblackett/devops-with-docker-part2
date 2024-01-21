FROM golang:1.19

WORKDIR /usr/src/app

COPY . /usr/src/app/

#ENV REQUEST_ORIGIN=http://localhost:5000
#ENV REQUEST_ORIGIN=http://proxy:5000
ENV PORT=8080

RUN go build
RUN go test ./...

CMD ["./server"]