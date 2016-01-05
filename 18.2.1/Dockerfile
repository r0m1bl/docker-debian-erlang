# Erlang
FROM debian:8.2

RUN apt-get update

RUN apt-get install git erlang && apt-get clean

#RUN git clone git://github.com/rebar/rebar.git && cd rebar && ./bootstrap && mv rebar /usr/local/bin/rebar && cd .. && rm -rf rebar/

ENTRYPOINT ["/bin/bash"]