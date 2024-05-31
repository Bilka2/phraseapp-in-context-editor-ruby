FROM ruby:3.2.1
WORKDIR /phraseapp-demo
COPY Gemfile .
COPY Gemfile.lock .
RUN gem update bundler && bundle install

# in examples/demo/: build the container
# `docker build -t phraseapp-demo .`
# in examples/demo/: start the container
# `docker run --rm -it -p 3010:3000 --mount type=bind,source=.,target=/phraseapp-demo phraseapp-demo bash`
# in the bash in the container: start the rails server
# `rails s -p 3000 -b '0.0.0.0'`
# on the host: open localhost:3010
