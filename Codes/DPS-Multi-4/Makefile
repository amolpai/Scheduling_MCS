CC = gcc
CFLAG = -g -Wall

all: test

test: auxiliary_functions.o check_functions.o processor_functions.o scheduler_functions.o driver.o
	$(CC) $(CFLAG) -o test auxiliary_functions.o check_functions.o processor_functions.o scheduler_functions.o driver.o -lm
	
driver.o: driver.c
	$(CC) $(CFLAG) -c driver.c

scheduler_functions.o: scheduler_functions.c
	$(CC) $(CFLAG) -c scheduler_functions.c

processor_functions.o: processor_functions.c
	$(CC) $(CFLAG) -c processor_functions.c

check_functions.o: check_functions.c
	$(CC) $(CFLAG) -c check_functions.c

auxiliary_functions.o: auxiliary_functions.c
	$(CC) $(CFLAG) -c auxiliary_functions.c

clean:
	rm -f *.o test
