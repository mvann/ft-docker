FROM ruby
RUN apt-get update &&\
	apt-get install -y sqlite3 &&\
	apt-get install -y nodejs
RUN gem install rails &&\
	gem install bundler
RUN mkdir /opt/app
WORKDIR /opt/app
ONBUILD ADD app /opt/app
ONBUILD RUN bundle install
ONBUILD RUN bundle exec rake db:setup
ONBUILD RUN bundle exec rake db:migrate
