# Lab Report
## Techinical Issue 
### Installation
No issue was encountered during the installation.
### JPA coding
#### -Stack overflow upon assertThat() returns False
When the code line 75 in the MainTest.Java is executed, the program determines that the elements don't match, thus creating an error message by calling the toString() method. However, I used Lombok to auto-generate toString() method and since the CreditCard class the Bank Class has a bidirectional mapping, this toString() method creates an infinite loop.
The issue is firstly solved by writing my own toString() method and later by passing the test, thus not calling the toString() method in the first place.
#### -Bank's card set doesn't match the expected value
When the code line 75 in the MainTest.Java is executed, the program determines that the elements don't match. A toString() call reveals both set (the tested set is bank's card set and the expected set is the set of two credit cards) have the same elements.
Further inspection shows 

## Github Link
https://github.com/CeruleanG/dat250-jpa-example
