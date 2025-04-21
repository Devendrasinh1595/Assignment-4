# Assignment-4
# Task 1
try:
 file1=open('sample.txt','r')
 reading_file1=file1.read()
 print(reading_file1)
 file1.close()
except FileNotFoundError :
    print("Error: ")
finally :
    print("The file 'sample.txt' was not found. ")

# Task 2
a=input('Enter text to write to the file: ')
file1=open('output.txt','w')
writing_file1=file1.write(a)
print(writing_file1)
file1.close()
file2=open('output.txt','a')
appending_file2=file2.write('\nLearning file handling in Python.')
print(appending_file2)
file2.close()
file3=open('output.txt','r')
reading_file3=file3.read()
print(reading_file3)
file3.close()
