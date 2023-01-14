# First pipe
## count file on usr bin
ls -l /usr/bin/ | wc -l

## save output on a new file
ls -l /usr/bin/ | wc -l > new_file.txt

## double ampersand
ls -l /usr/bin/ && touch new_file.txt

## object assignment
strin=$'first line\nsecond line\nthird line' 
echo "$strin"

# Second pipe
echo "$strin" > newText.txt
cat newText.txt | sort -r | less
cat newText.txt | grep th > match.txt

## append
echo "love" > text2.txt
echo "Entin" >> text2.txt

## history log
history
history | head -n 4
history | tail -n 4
history | grep echo