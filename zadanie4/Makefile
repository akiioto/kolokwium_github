CC = g++

OBJS = main.o
EXEC = myProgram

$(EXEC): $(OBJS)
	$(CC) $+ -o $@
	echo hello: zbudowano!

%.o: %.cpp
	$(CC) -c $<

main.o: address.h employee.h

clean:
	rm -f *~
	rm -f *.bak
	rm -f $(EXEC) $(OBJS)

.PHONY: clean
