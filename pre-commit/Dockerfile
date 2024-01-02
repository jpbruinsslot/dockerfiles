FROM python:3.11
RUN apt update || true && apt install -y git --no-install-recommends
RUN pip install pre-commit
WORKDIR /usr/src/app
RUN sh -c "git config --global --add safe.directory /usr/src/app"
ENTRYPOINT [ "pre-commit" ]
CMD []
