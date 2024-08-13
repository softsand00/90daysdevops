## Day 3 Task: Basic Linux Commands
1. ### To view what's written in a file
    cat
2. ### To change the access permissions of files.
   chmod
3. ### To check which commands you have run till now.
    history
4. ### To remove a directory/ Folder.
    rmdir - To remove empty directory
    rm -r - To remove directory with folders
5. ### To create a fruits.txt file and to view the content.
     touch - to create file
     cat - to view
6. ### Add content in devops.txt (One in each line) - Apple, Mango, Banana, Cherry, Kiwi, Orange, Guava.
   #### This command creates or overwrites devops.txt with the list of fruits, each on a new line.
   echo -e "Apple\nMango\nBanana\nCherry\nKiwi\nOrange\nGuava" > devops.txt
   #### To append the content to the existing file without overwriting it, use:
   echo -e "Apple\nMango\nBanana\nCherry\nKiwi\nOrange\nGuava" >> devops.txt
7. ### To Show only top three fruits from the file.
   head -n 3 filename
8. ### To Show only bottom three fruits from the file.
   tail -3 filename
9. ### To create another file Colors.txt and to view the content.
   vim Colours.txt 
   cat Colours.txt
11. ### Add content in Colors.txt (One in each line) - Red, Pink, White, Black, Blue, Orange, Purple, Grey.
     echo -e "Red\nBlue\nGreen\nYellow\nPurple\nOrange\nPink" > Colors.txt
10. ### To find the difference between fruits.txt and Colors.txt file.
    diff fruits.txt Colors.txt
11. ### To find the Same between fruits.txt and Colors.txt file.
    *1 Sort both the files
    sort fruits.txt -o fruits.txt
    sort Colors.txt -o Colors.txt
    *2 Find common
    comm -12 fruits.txt Colors.txt

