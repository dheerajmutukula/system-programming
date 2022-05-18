CC = g++
BIN = bin/
OBJ = obj/
INC = include/
SRC = src/
CFLAG = -c
OFLAG = -o
all:clean build-server build-client

build-server: ${OBJ}func.o
	${CC} ${OFLAG} ${BIN}server04 ${SRC}server.cpp ${OBJ}func.o
$(OBJ)func.o:
	${CC} ${CFLAG} ${OFLAG} ${OBJ}func.o ${SRC}func.cpp
build-client:
	${CC} ${OFLAG} ${BIN}client04 ${SRC}client.cpp
start-server:
	./${BIN}server04
start-client:
	./${BIN}client04
clean:
	rm ${OBJ}func.o ${BIN}server04 ${BIN}client04
