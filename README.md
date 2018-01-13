# Defensive-Security-System
Reference monitor to maintain data integrity of files 
## Synopsis
1. A Reference Monitor which will keep two copies of every file incase it is incorrectly written. The valid copy is used for reading and the other one is used for writing. On closing the file, if a file copy is invalid then it is discarded and if both the file copies are valid, the older one is discarded. The system was implemented using locks to support multithreading
2. The system was developed using the security layer functionality in Repy V2 which is a subset of Python and tested with numerous attack cases
