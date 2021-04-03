FROM tarantool/tarantool

RUN apk add musl-dev gcc
RUN cd /usr/local && \
	tarantoolctl rocks install tarantool-lsp && \
	cp -r .rocks/share/tarantool/tarantool-lsp /usr/local/tarantool-lsp && \
	cd /usr/local/bin && wget https://raw.githubusercontent.com/tarantool/lua-lsp/master/bin/tarantool-lsp && \
	chmod +x tarantool-lsp