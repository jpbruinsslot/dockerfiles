FROM alpine:3.20

RUN apk add --no-cache \
    bcc-doc \
    bcc-tools \
    bpftrace \
    bpftrace-doc \
    bpftrace-tools \
    bpftrace-tools-doc

ENTRYPOINT ["/usr/bin/bpftrace"]
CMD []
