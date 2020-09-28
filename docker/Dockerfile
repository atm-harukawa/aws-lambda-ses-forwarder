FROM node:12-alpine

# install curl, python tooling and other utilities
RUN apk add --update git curl python-dev py-pip screen gpgme maven openjdk8 && pip install --upgrade pip && \
	rm -rf /var/cache/apk/*

# install yarn
RUN curl -o- -L https://yarnpkg.com/install.sh | sh
ENV PATH /root/.yarn/bin:$PATH
