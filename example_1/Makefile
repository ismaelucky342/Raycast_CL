CC = gcc
CFLAGS = -Wno-implicit-int
LIBS = -lGL -lGLU -lglut -lm

SRC = raycast.c
OBJ = $(SRC:.c=.o)

TARGET = raycast

all: $(TARGET)

$(TARGET): $(OBJ)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJ) $(LIBS)

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJ)

fclean: clean
	rm -f $(TARGET)

re: fclean all