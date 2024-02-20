CC = gcc
CFLAGS = -Wall -Wextra -std=c11
SRCS = $(wildcard *.c)
OBJS = $(SRCS:.c=.o)
TARGET = calculator

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) -o $@ $^

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJS) $(TARGET)