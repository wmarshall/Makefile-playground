
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
