# Parametry prekladace.
CFLAGS=-Wall -ansi -O9

PROGNAME=mandelbrot

all:	$(PROGNAME)

clean:
	rm *.o
	rm $(PROGNAME)

# Pravidlo pro slinkovani vsech objektovych souboru a vytvoreni
# vysledne spustitelne aplikace.
$(PROGNAME):	$(PROGNAME).o
	$(CC) -o $@ $(LDFLAGS) $<

# Pravidlo pro preklad kazdeho zdrojoveho souboru do prislusneho
# objektoveho souboru.
%.o:	%.c
	$(CC) $(CFLAGS) -c $< -o $@

