ARG version
FROM almalinux:${version:-9}
ENV course="AWS devops" \
    trainer="siva" \
    duration="120HRS"
ARG USERNAME=SIVAKUMAR
ENV USERNAME=$USERNAME
RUN echo "Hello ${USERNAME}, image version:${version}"
 CMD ["sleep","100"]