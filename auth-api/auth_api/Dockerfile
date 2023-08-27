FROM golang:1.9-alpine

COPY . /app
WORKDIR /go/src/app
RUN apk --no-cache add curl git && \
    curl https://raw.githubusercontent.com/golang/dep/master/install.sh | sh



COPY --from=build

RUN dep ensure \
    go build -o auth-api

CMD /go/src/app/auth-api

