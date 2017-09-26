ERTS_INCLUDE_DIR = $(shell erl -noshell -s init stop -eval "io:format(\"~s/erts-~s/include/\", [code:root_dir(), erlang:system_info(version)]).")
all:
	mkdir -p ../priv
	gcc -shared -o ../priv/b64fast.so -fPIC -I $(ERTS_INCLUDE_DIR) b64fast.c
