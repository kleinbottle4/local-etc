CC     = tcc
OBJ    = main.c
OUT    = a.out
CMD    = $(CC) $(OBJ) -o $(OUT)


$(OUT) : $(OBJ)
	$(CMD)

clean :
	rm $(OUT)

loop:
	echo $(OBJ) | entr -s "$(CMD)"
