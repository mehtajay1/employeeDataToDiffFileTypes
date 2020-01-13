# employeeDataToDiffFileTypes
"1. Implement Employee class with following specification          String firstName         String lastName          Date    dateOfBirth         double        experience  

2. Implement MyCollection class with the following specification         Array of 300 entries of Employee class         writeCounter         readCounter         The following methods to be syncronized          add(Employee) -> new element should be added at writeCounter, writeCounter should be increment after every insert          Employee get() -> element should be readCounter, readCounter should be incremented after every read operation  

3. Define a interface MyFileHandler with following methods  
i. read 
ii. write

4. Declare CSVFileHandler, XMLFileHandler, JsonFileHandler classes that implements MyFileHandler  
i.   CSVFileHandler should have ability to read and write data in CSV        
ii.  XMLFileHandler should have ability to read and write data in XML     
iii. JsonFileHandler should have ability to read and write data in JSON 

5. Generate three data files and each file containing 100 records. File one should be CSV format, file should be in XML format and file three should be in JSON format  

6. Develop a controller class MyController with the following logic    
i. Create three threads and allocate one threads each for reading data from CSV, XML and JSON   
ii. Each thread reads record by record and insert into MyCollection class    
iii. Main thread that has created three threads should wait for all threads to finish  

7. Once the read finishes, print the count of elements from MyCollection, it should be 300 and write counter should be properly updated to 300  

8. Create three threads to write data from MyCollection with the following specifications  
i. Each thread reading one record from MyCollection, read method should return the value and increment the counter   
ii. Thread 1 should write record in CSV        
iii. Thread 2 should write records in XML     
iv. Thread 3 should write records in JSON       
v. Once record is wirtten to the file thread should seek next record from MyCollection       
vi. Each thread should finish reading after 100 records        
vii. Files should not have duplicate records and should not have more than 100 records "
