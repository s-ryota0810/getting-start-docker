#FROM: Dockerイメージのベースとなるイメージを指定する
FROM golang:1.13

#RUN: Dockerイメージビルド時に、コンテナ内で実行するコマンドを定義する
RUN mkdir /test

#COPY: ホストマシンからコンテナ上へコピーする時などに使う
COPY main.go /test

#CMD: コンテナ内で実行するプロセスを指定、コンテナ起動時に一度だけ実行される
#アプリケーションそのものを動作させるイメージ
#空白を配列で表現する
CMD ["go", "run", "/test/main.go"]