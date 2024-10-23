# Counting Word Occurrences in UNIX

## Question
Which of the following UNIX commands will correctly count the occurrences of the word "example" in a file named "textfile.txt"?

1. `grep 'example' textfile.txt | wc -l`
2. `grep -c 'example' textfile.txt`
3. `grep -o 'example' textfile.txt | wc -l`
4. `find 'example' textfile.txt`

## Options
1. **`grep 'example' textfile.txt | wc -l`**  
   - **Explanation**: This command counts the number of lines containing the word "example." It will give a count for lines where "example" appears but not the total occurrences if the word appears multiple times on the same line.

2. **`grep -c 'example' textfile.txt`**  
   - **Explanation**: This command counts the number of lines that contain the word "example," not the total number of occurrences of the word itself.

3. **`grep -o 'example' textfile.txt | wc -l`**  
   - **Explanation**: This is the correct command. It prints each occurrence of the word "example" on a new line and then counts those lines, resulting in the total number of occurrences.

4. **`find 'example' textfile.txt`**  
   - **Explanation**: This command is incorrect because `find` is used for searching for files and directories, not for searching content within files. 

## Correct Answer
**Option 3: `grep -o 'example' textfile.txt | wc -l`**
