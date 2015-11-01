##Problem 1

How would you print just the 10th line of a file?

For example, assume that file.txt has the following content:

```
Line 1
Line 2
Line 3
Line 4
Line 5
Line 6
Line 7
Line 8
Line 9
Line 10
```

 Your script should output the tenth line, which is:

```
	Line 10
```

```Bash
	sed "10d;q" file.txt

	awk 'END{print}' file.txt
```


##Transpose File

Given a text file file.txt, transpose its content.

You may assume that each row has the same number of columns and each field is separated by the ' ' character.

 For example, if file.txt has the following content:

```
	name	age
	Alice	21
	Ryan	30
```

Output the following:

```
	name alice ryan
	age 21 30
```

##Valid Phone Numbers

Given a text file file.txt that contains list of phone numbers (one per line), write a one liner bash script to print all valid phone numbers.

You may assume that a valid phone number must appear in one of the following two formats: (xxx) xxx-xxxx or xxx-xxx-xxxx. (x means a digit)

You may also assume each line in the text file must not contain leading or trailing white spaces.

For example, assume that file.txt has the following content:

```
	987-123-4567
	123 456 7890
	(123) 456-7890
```

 Your script should output the following valid phone numbers:

```
	987-123-4567
	(123) 456-7890
```