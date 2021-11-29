FROM openjdk:14-alpine

ARG VERSION=5.3

RUN wget https://www.languagetool.org/download/LanguageTool-${VERSION}.zip && \
    unzip LanguageTool-${VERSION}.zip && \
    rm LanguageTool-${VERSION}.zip

WORKDIR /LanguageTool-${VERSION}

ENTRYPOINT ["java", "-jar", "languagetool-commandline.jar"]
CMD []
