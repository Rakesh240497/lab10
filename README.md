# lab10


1. The aim of the lab is to print the output in a out or err extension files rather than on the terminal. 
2. I have used lab7 program as a startup and edited the code according to the requirement given in the lab. 
3. First to create files with process, I have created to arrays for extensions of the files which are ".out" and ".err"
4. Than to hold the complete file name i have created to more array variables for out and err with the size of 10. 
5. Using the getpid() funtion i have assing the process id to an integer variable ppid = getpid(). 
6. Than using the sprintf i have created the file name with ppid as a prefix and extensions as suffix. 
7. In addition to these i have declared two file descriptors for outfile and errfile. 
8. Using the open function i have created the files for out and err functionalites with 0755 permission standard. 
9. If there is any error while creating these file an error message will be printed accordingly. 
10. Once the files creation is succesfull i have called dup2() function to assign the functionalities of standard stdout and stderr. 
11. In a sample.txt file i have wrote the commands and this file will be given to the program as a argv variable. 
12. The program exucutes the commands given in the sample.txt file and creates the files with process id along with proper extensions. And writes the output to these file accordingly instead of the terminal. 
