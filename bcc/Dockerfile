# https://github.com/iovisor/bcc/blob/master/INSTALL.md#alpine---binary
FROM alpine:3.20

RUN apk add --no-cache \
    bcc-tools \
    bcc-doc

# Set the working directory to where the tools are located
WORKDIR /usr/share/bcc/tools

# Make the directory available for PATH
ENV PATH="/usr/share/bcc/tools:${PATH}"

# Set a flexible entrypoint to execute tools dynamically
ENTRYPOINT ["/bin/sh", "-c"]
