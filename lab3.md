
## Lab3: Researching Commands

This report shows examples of different uses of the grep command.

## PART 1: expressions to search

A first grep command that can be used is the regular expression command, which follows the format `grep "[pattern]\{n occurrences\}...." <file.txt>`, and prints all the lines that follow the pattern in quotes. 

Two examples of this are shown below, using two different text files:

``` 
$ grep "[a-n]\{6\}[n-z]" Kiosks_for_court_forms.txt 

lawyer, but it also might improve efficiency in the courts because
used the free system, located in public buildings throughout Orange
Cohen said the system proves the benefit of technology tailored 
```
```
$ grep "[a-i]\{6\}[n-z]" diversity_priorities.txt 

neither real dedication to making it happen nor any real
uncomfortable issues, give up power and make difficult financial
not achieved without certain difficulties. Diversity "pioneers"
difficult conversations.
```
## PART 2: search with line numbers

Another grep command that can be used is the search command that also outputs the line(s) and line number(s) in which the word is found. This command follows the format `grep -n "word" <file.txt>`, and prints all the lines and line numbersm that contain the word in quotes. 

Two examples of this are shown below, using two different text files:

```
$ grep -n "paperwork" Kiosks_for_court_forms.txt 

6:System to help the uninitiated fill out minor paperwork could go
21:out paperwork for restraining orders, eviction defense,
66:nervous with that kind of paperwork, and you want to do it right,"
```
```
$ grep -n "each" diversity_priorities.txt 

72:era. The thoughts and observations of each group are reported
172:members tend to embrace the belief that each person who needs a
225:excuses. We realize that diversity can help programs reach clients
345:authentic commitment to diversity throughout each program is
416:charging certain staff members to "reach out" to others to overcome
466:policies that implement diversity goals are adopted throughout each
470:strategies for reaching severely marginalized communities and our
502:participants include at least 1-2 staff from each program; it is
529:policies. They hire individuals to act as leaders, teachers and
```
## PART 3: search number of times

Another grep command that can be used is the search command that also outputs the number of time that the word is found. This command follows the format `grep -c "word" <file.txt>`, and prints an integer of the number of times the words occur. 

Two examples of this are shown below, using two different text files:

```
$ grep -c "easy" Kiosks_for_court_forms.txt 

4
```
```
$ grep -c "in" diversity_priorities.txt 

235
```
## PART 4: search number with surrounding lines

Another grep command that can be used is the search command that outputs the searched word and surrounding lines. This command follows the format `grep -C <n lines. "word" <file.txt>`, and prints the surrounding inputted number of lines around each instance of the word.

Two examples of this are shown below, using two different text files:


```
$ grep -C 2 "changes" diversity_priorities.txt 

authentic commitment to diversity throughout each program is
essential. A core group can begin the work, but structural and
programmatic changes -- mentoring, opportunities to talk about real
problems and see solutions implemented, power sharing, diverse
boards of Directors, new definitions of leadership --will be
```
```
$ grep -C 2 "2000" Kiosks_for_court_forms.txt 

the forms, which are printed out when completed, are easy to read
and are being filled out correctly, the study found.
Since the program started in 2000, more than 6,000 people have
used the free system, located in public buildings throughout Orange
County.
```



Source Used: ChatGPT, Accessed through https://chat.openai.com/ on 5/24/23

input: please tell me some interesting and fun grep commands

output: ChatGPT
Sure! Here are some interesting and fun grep commands that you can try:

Search for a specific word in a file:
grep "word" file.txt

Case-insensitive search:
grep -i "word" file.txt

Search for a word and display the line number:
grep -n "word" file.txt

Search for a word in multiple files:
grep "word" file1.txt file2.txt

Search for a word recursively in a directory:
grep -r "word" directory/

Search for a word excluding a specific file or directory:
grep "word" --exclude-file=exclude.txt

Search for a word and display surrounding lines:
grep -C 2 "word" file.txt

Display only the matched word, ignoring the rest of the line:
grep -o "word" file.txt

Count the number of occurrences of a word:
grep -c "word" file.txt

Use regular expressions to search for patterns:
grep "pattern[0-9]" file.txt
Remember, these are just a few examples, and grep is a powerful tool with many options and use cases. You can explore its manual page (man grep) to learn more about its capabilities.
