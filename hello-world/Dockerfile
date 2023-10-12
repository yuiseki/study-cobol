FROM ubuntu:latest

RUN apt-get update
RUN apt-get install -y gnucobol

WORKDIR /app
COPY main.cbl .
RUN cobc -x ./main.cbl
CMD ["./main"]
