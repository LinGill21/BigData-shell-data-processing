# Bash Cheatsheet
* Curl to a file
```bash
curl "https://www.poetryfoundation.org/poems/42891/stopping-by-woods-on-a-snowy-evening" -o frost.txt
```
* Transform each space ' ' into a return character '\12'
```bash
tr ' ' '\12' < filetoRead.txt
```
* Pipe the output to sort
```bash
tr ' ' '\12' < filetoRead.txt | sort
```
* Pipe the sorted output to uniq -c to count 
```bash
tr ' ' '\12' < filetoRead.txt | sort | uniq -c
```
* Pipe the reduced output to sort with -nr flag
```bash
tr ' ' '\12' < filetoRead.txt | sort | uniq -c | sort -nr
```
* Redirect the output to result.txt 
```bash
tr ' ' '\12' < filetoRead.txt | sort | uniq -c | sort -nr >result.txt
```
* the bash up arrow will bring up the previous cmd
* sort -n **sort numeric** or  compare according to string numerical value
* sort -r **sort reversed** or reverse the result of comparisons
* a single letter flag gets a single dash if the flag is a woord it will get two dashes
* bash redirect: cmd>file.txt will send output to a file
* bash redirect and append: cmd>file.txt will concatenate output to a file
