You will create a small text file and practice:
- Creating a file
- Writing text to a file
- Appending new lines
- Reading the file back


## Guidelines
Follow these rules while creating your practice note:

- Create a file named `notes.txt`
- Write 3 lines into the file using **redirection** (`>` and `>>`)
- Use **`cat`** to read the full file
- Use **`head`** and **`tail`** to read parts of the file
- Use **`tee`** once to write and display at the same time
- Keep it short (8–12 lines total in the file)

Suggested command flow:
1. `touch notes.txt` - create a file 
2. `echo "Line 1" > notes.txt` - add text to it using aapend 
3. `echo "Line 2" >> notes.txt` - add new lines in file
4. `echo "Line 3" | tee -a notes.txt` - adds new line and displays it 
5. `cat notes.txt` - read the file
6. `head -n 2 notes.txt` - displays first 2 lines from file
7. `tail -n 2 notes.txt` - displays bottom 2 lines from file

---

## Resources
Use these docs to understand the commands:

- `touch` (create an empty file) 
- `cat` (read full file) 
- `head` and `tail` (read parts of a file) 
- `tee` (write and display at the same time)
- (single append ">") Deletes everything inside the file and replaces it with the new text
- (Double append ">>") Adds to the end of the file 

