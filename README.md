# shell-data-processing

## Retrieve text from URL
- I have used curl "url" -O "data.txt" command to retrieve the text from url "http://shakespeare.mit.edu/romeo_juliet/full.html" and store the result in data.txt file.

## Process Text Data
- Command "tr ' ' '\12' < data.txt" is used to map each line into individual words.
- Command "tr ' ' '\12' < returnedfile | sort" is used to sort individual words.
- Command "tr ' ' '\12' < returnedfile | sort | uniq -c" is used to count the unique words from the sorted result.
- Command "tr ' ' '\12' < returnedfile | sort | uniq -c | sort -nr" is used to sort in reverse order -r will do in reverse order.
- Commapd "tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt" is used to store the output in result.txt file.
- hit the up arrow in bash shell is used to get the previous executed command.
- "-n" flag is used to sort by numeric value
- "-r" flag is used to sort the data in reverse order
