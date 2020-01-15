CC = g++
LFLAGS = -lm
OBJS = main.o employee.o address.o
EXEC = myProgram

$(EXEC): $(OBJS)
	$(CC) $(LFLAGS) $(OBJS) -o $(EXEC)
	echo myProgram: zbudowane!

main.o: employee.h address.h
	$(CC) -c main.cpp

employee.o: employee.cpp
	$(CC) -c employee.cpp

address.o: address.cpp
	$(CC) -c address.cpp

clean:
	rm -f *~ *.bak
	rm -f $(EXEC) $(OBJS)

.PHONY: clean
