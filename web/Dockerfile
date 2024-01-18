FROM ubuntu:latest
#install go with apt-get
RUN apt-get update && apt-get install -y golang
COPY . .
#build the go app
RUN go build dispatcher.go
#run the go app
CMD ["./dispatcher"]


#2eme facon
#FROM golang:alpine AS builder
#COPY dispatcher.go .    
#RUN go build dispatcher.go

#FROM alpine
#COPY --from=builder go/dispatcher .
#COPY static static 
#CMD ["./dispatcher"]