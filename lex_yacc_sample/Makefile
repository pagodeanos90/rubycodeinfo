CC=gcc

grammar: lex.l parse.y y.tab.h
	lex lex.l
	yacc -d parse.y
	$(CC) -c lex.yy.c y.tab.c
	$(CC) -o parser lex.yy.o y.tab.o -ll

clean:
	rm *.o 

