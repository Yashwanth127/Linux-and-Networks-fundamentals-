# create practice folder
mkdir day2-practice
cd day2-practice

# create files
touch file1.txt file2.txt file3.txt

# check files
ls

# copy file
cp file1.txt file1-copy.txt

# copy multiple files into folder
mkdir backup
cp file1.txt file2.txt backup/

# move file
mv file3.txt renamed-file3.txt

# move file into folder
mv renamed-file3.txt backup/

# delete file
rm file2.txt

# check final structure
ls
ls backup
