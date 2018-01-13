# Defensive-Security-System
Reference monitor to maintain data integrity of files 
## Synopsis
1. A Reference Monitor which will keep two copies of every file incase it is incorrectly written. The valid copy is used for reading and the other one is used for writing. On closing the file, if a file copy is invalid then it is discarded and if both the file copies are valid, the older one is discarded. The system was implemented using locks to support multithreading
2. The system was developed using the security layer functionality in Repy V2 which is a subset of Python and tested with numerous attack cases
### Attack Case Explanation
1. Attack Case 1 : It checks if valid data write to a file is successful i.e. checks if the accuracy of the system is not compromised.
2. Attack Case 2 : It checks if an existing file is reopened successfully i.e checks if the accuracy of the system is not compromised.
3. Attack Case 3 : It checks if the system prevents saving of invalid data in a file when the file is closed i.e. checks if the security of the system is not compromised.
4. Attack Case 4 : It checks if the empty file condition of writing valid data SE by default in a file is satisfied when a new file is created i.e. checks if the accuracy of the system is not compromised.
5. Attack Case 5 : It checks if data is read from the valid copy/data is written into the other copy when valid data is written and the file is not closed i.e. checks if the security of the system is not compromised.
6. Attack Case 6 : It checks if data is read from the valid copy/data is written into the other copy when invalid data is written and the file is not closed i.e. checks if the security of the system is not compromised.
7. Attack Case 7 : It checks if the system is allowing to perform a simple write operation i.e. checks if the accuracy of the system is not compromised.
8. Attack Case 8 : It checks if the system is allowing to perform a simple read operation i.e. checks if the accuracy of the system is not compromised.
9. Attack Case 9 : It checks if the system handles writing in multiple files simultaneously i.e. checks if the accuracy of the system is not compromised.
10. Attack Case 10 : It checks if the system handles writing in multiple files simultaneously i.e. checks if the accuracy of the system is not compromised. 
