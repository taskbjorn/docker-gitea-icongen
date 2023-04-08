FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y \
        build-essential \
        git \
        npm && \
    apt-get clean

RUN git clone https://github.com/go-gitea/gitea /gitea && \
    cd /gitea && \
    git checkout f7e7477c45b064c220c1dc87afec89b40c396312

WORKDIR /gitea

CMD make generate-images