#LIBS  = -lkernel32 -luser32 -lgdi32 -lopengl32
LIBES = 
CFLAGS = -Wall
CC = gcc

# Should be equivalent to your list of C files, if you don't build selectively
SRCS = $(wildcard *.c)
OBJS = $(patsubst %.c,%,$(SRCS))

#
#all: $(SRC)
#	$(CC) $(CFLAGS) $< -o $@ $(LIBS)

all: $(SRCS:.c=)

.c:
	$(CC) $(CFLAGS) $< -o $@

hello: 
	$(CC) $(CFLAGS) hello.c -o hello.o

#
clean:
	rm *.o
