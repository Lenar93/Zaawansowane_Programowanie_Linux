GCC=i686-crosscompilator

all: hello main
hello:
	$(GCC) Include/hello.c -shared -o libhello.so
main: hello
	$(GCC) ./Prog1/main.c -I ./Include -L . -lhello -o main
