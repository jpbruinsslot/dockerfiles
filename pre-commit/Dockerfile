FROM python:3.11
RUN apt-get update || true && apt-get install -y git --no-install-recommends && apt-get clean
RUN pip --no-cache-dir install pre-commit==3.8.0
WORKDIR /usr/src/app
RUN sh -c "git config --global --add safe.directory /usr/src/app"
ENTRYPOINT [ "pre-commit" ]
CMD []
