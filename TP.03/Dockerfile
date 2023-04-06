FROM ubuntu:latest AS lourde

WORKDIR /lourd

RUN touch patate.txt
RUN apt update -y
RUN apt install apache2 -y

CMD service apache2 start && sleep infinity




FROM alpine:latest AS legere

COPY --from=lourde ./lourd /leger
