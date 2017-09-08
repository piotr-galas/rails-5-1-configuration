FROM ruby:2.4.0

RUN apt-get update -qq
RUN apt-get install apt-transport-https

RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list
RUN curl -sL https://deb.nodesource.com/setup_7.x | bash -
RUN apt-get update -qq

RUN apt-get install -y build-essential libpq-dev  yarn nodejs

WORKDIR /rails_app

ENV BUNDLE_PATH=/rails_app_gems
ENV RAILS_ENV=development