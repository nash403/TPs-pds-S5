.PHONY : clean fclean test all

CC = gcc
CFLAGS = -Wall -Werror -B -ansi -pedantic
CFLAGS += -D_XOPEN_SOURCE=500
CFLAGS += -g

all : do

do: do.c makeargv.h
	$(CC) $(CFLAGS) -o $@ makeargv.c $<
	

test: clean
	bash sessionTest.sh


clean :
	rm -f *.o *~

fclean : clean
	rm -f do
