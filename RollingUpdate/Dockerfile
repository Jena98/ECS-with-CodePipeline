FROM alpine:latest

RUN mkdir /lib64 && \
ln -s /lib/libc.musl-x86_64.so.1 /lib64/ld-linux-x86-64.so.2 

COPY ./app /root

EXPOSE 8000

WORKDIR /root

ENTRYPOINT ["/bin/sh", "-c"]

CMD ["./app"]
