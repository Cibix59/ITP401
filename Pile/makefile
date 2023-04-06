CC=gcc
CFLAGS=-Wall #-Wextra
LDFLAGS=
VERSION_P=tab
SOURCES=Element.c cellule.c Pile_$(VERSION_P).c Pile_test.c
OBJECTS=$(SOURCES:.c=.o)
EXECUTABLE=main

all: $(SOURCES) $(EXECUTABLE)

$(EXECUTABLE): $(OBJECTS)
	$(CC) $(LDFLAGS) $(OBJECTS) -o $@

.c.o:
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJECTS) $(EXECUTABLE)