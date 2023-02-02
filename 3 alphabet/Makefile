
alphabet-simple.txt:
	echo "abcdefghijklmnopqrstuvwxyz" > alphabet-simple.txt

alphabet-expansion.txt:
	echo "abcdefghijklmnopqrstuvwxyz" > $@

alphabet-prerequisites.txt: alphabet-simple.txt alphabet-expansion.txt
	cat $^ > $@

clean-not-phony:
	rm alphabet-*.txt

.PHONY: clean
clean:
	rm alphabet-*.txt

ALPABET_ONE_BY_ONE:=alphabet-one-by-one.txt

.PHONY: a b c d e f g h i j k l m n o p q r s t u v w x y z
a:
	echo "a" >> $(ALPABET_ONE_BY_ONE)
b: a
	echo "b" >> $(ALPABET_ONE_BY_ONE)


$(ALPABET_ONE_BY_ONE): a b c d e f g h i j k l m n o p q r s t u v w x y z

