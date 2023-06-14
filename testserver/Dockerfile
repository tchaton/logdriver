FROM  golang:1.20.4

COPY . /go/src/github.com/monmohan/testserver
RUN cd /go/src/github.com/monmohan/testserver && go get && go build --ldflags '-extldflags "-static"' -o /usr/bin/testserver
EXPOSE 9000
CMD ["/usr/bin/testserver"]

