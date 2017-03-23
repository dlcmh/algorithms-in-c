CC = cc
CFLAGS = -Wall -g
COMPILE = $(CC) $(CFLAGS) -c
OBJFILES := $(patsubst %.c,%.o,$(wildcard *.c))
PROG_NAME = Main

all: myprog

myprog: $(OBJFILES)
	$(CC) -o $(PROG_NAME).app $(OBJFILES)

%.o: %.c
	$(COMPILE) -o $@ $<

clean:
	rm -f *.o $(PROG_NAME).app
