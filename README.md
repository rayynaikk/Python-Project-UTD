# Python-Project-UTD
This project uses concepts like Polymorphism,  Inheritance, ClassMethod were implemented. datetime and time packages were used from python libraries.


1
Object Oriented Programming: Scooter Rental shop
University of Texas at Dallas


2

UTD Scooter Rental Shop
This project uses intermediate level python programming. Concepts like Polymorphism, 
Inheritance, ClassMethod and basic File operations were implemented.
It starts with definition of Parent Class "AutoDealer" which consists of init and repr constructors 
alongwith some instance methods which will be used by the child classes. Child classes for this 
parent are "ScootRent" and "ScootReturn". All the user inputs like name, quantity, service 
options and time period are taken in the main() class. Based on these inputs and choice of 
services, we make decisions to create objects from required child class and perform operations. 
datetime and time packages were used from python libraries.

3

Complete procedure explained:

Parent Class - AutoDealer
Consists of a global variable total which indicates the total number of scooters available in 
stock. Following the problem statement, we initialise it as "7". Method "setReturnDatetime" is 
defined to set the order time and calculate the return window based on the rental duration 
selected by user. This duration can be hourly/daily/weekly. This method returns return date 
and time. Method "get_price" checks for the quantity of scooters requested and provides price 
discount if quantity is more than 2. This method returns the final price of the transaction. 
Method "AvailableCount" returns the available count of the scooters in stock after any 
transaction is done. Method "returned" calculates the total after returning a scooter. "init" and 
"repr" constructors are used to initialise instance variables and print return valules for the class. 
Apart from this, a classmethod has been defined to update the global variable "total" 
depending on the argument "oper", which lets the method know if the count to be increased or 
decreased.

Child Class - ScootRent

This class consists of "init" & "repr" constructors which initialise the class variables and returns 
string value for invoice generated.

Child Class - ScootReturn

This class also consists of "init" & "repr" constructors which initialise the class variables and 
returns string value for message to be displayed during return.
Function pricePoint
This function sets the price rates according to hourly/daily/weekly option selected by user.

Calling Class - main()

Since it has to be a continuous interaction while(True) was used. Displays a welcome message, 
showing customer the options for service required. Choice input is taken from the customer 
into variable "Choice". If the choice is "3" which means exit we break the loop using break. If 
any other options, we take customer Name, Duration category, duration and quantity as inputs 
to process the data and perform necessary operations. Object of ScootRent is created. Since 
maximum of 5 scooters can be rented, quantity variable is checked for condition. If conditions 
are satisfied, we append the invoice message into a text file "Customername_timestamp" 
located at the same location where project is situated. Total available count of scooters is 
updated using class method and displayed on the console. If scooter has to be returned, object 
of ScootReturn is created and after taking user inputs for name, duration and quantity, total 
count of available stock is updated. repr out is printed on the console consisting of a thankyou 
message.

