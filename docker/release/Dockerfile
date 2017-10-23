FROM jlang/todobackend-base:latest
LABEL maintainer="jlang"

# copy artifats
COPY target /wheelhouse

# install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse