FROM golang:1.16.5-alpine

WORKDIR /server

COPY . .

ENV GO111MODULE=on

RUN apk add git

# go get
RUN go get github.com/labstack/echo/...
RUN go get github.com/pilu/fresh

CMD ["fresh"]