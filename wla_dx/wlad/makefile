
CC?=egcs
LD?=egcs

CFLAGS?= -c -ansi -O3 -pedantic -Wall -DUNIX -DGB
LDFLAGS = 

CFILES = main.c
HFILES = main.h
OFILES = main.o

all: $(OFILES) makefile
	$(LD) $(LDFLAGS) $(OFILES) -o wlad ; strip wlad

main.o: main.c main.h makefile
	$(CC) $(CFLAGS) main.c


$(OFILES): $(HFILES)


clean:
	rm -f $(OFILES) core *~ wlad

install:
	make ; cp wlad /usr/local/bin
