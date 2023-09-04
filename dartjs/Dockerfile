From dart:3.1.0-sdk

RUN mkdir /app
COPY . /app
WORKDIR /app
RUN dart pub get
RUN dart compile exe /app/server.dart -o /app/bin/server
CMD [ "/app/bin/server" ]
