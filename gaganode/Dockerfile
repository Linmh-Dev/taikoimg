FROM ubuntu:18.04
RUN curl -o apphub-linux-amd64.tar.gz https://assets.coreservice.io/public/package/60/app-market-gaga-pro/1.0.4/app-market-gaga-pro-1_0_4.tar.gz && tar -zxf apphub-linux-amd64.tar.gz && rm -f apphub-linux-amd64.tar.gz && cd ./apphub-linux-amd64
RUN sudo ./apphub service remove && sudo ./apphub service install
RUN sudo ./apphub service start
RUN ./apphub status
RUN sudo ./apps/gaganode/gaganode config set --token=zuqzfxgfylebcwpc79c244ebe2380448
RUN ./apphub restart
