ARG Version
FROM almalinux:${Version:-8}
ARG Greeting="Hi"
ENV Greet=${Greeting}
RUN echo "$Greeting"
RUN echo "$Version"