# Erlang
FROM debian:8.2

RUN apt-get update

RUN apt-get install -y build-essential libncurses5-dev openssl libssl-dev fop xsltproc unixodbc-dev wget git &&\
	apt-get clean -y

RUN wget http://www.erlang.org/download/otp_src_18.2.1.tar.gz &&\
	tar zxvf otp_src_18.2.1.tar.gz &&\
	cd otp_src_18.2.1 &&\
	./configure && make && make install

RUN git clone git://github.com/nitrogen/nitrogen

#RUN git clone git://github.com/rebar/rebar.git && cd rebar && ./bootstrap && mv rebar /usr/local/bin/rebar && cd .. && rm -rf rebar/

ENTRYPOINT ["/bin/bash"]