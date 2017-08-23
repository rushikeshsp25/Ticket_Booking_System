# Ticket_Booking_System
Implemented in C++

This program is a implementation of Ticket Booking System using Doubly Circular Linked List. Data structures used in the program- Doubly Circular Linked List.

Why Dcll?
We know that in theatres more than 200 seats are there, Now if our head pointer points to the seat number ‘A1’ & user want to perform some operation with seat number ‘J1’ then it will be very much time consuming task ,as we need to traverse whole linked list from A1 to J7.

------------------------------------------->Space Left for Image <---------------------------------------------------------

Now when we use Doubly circular Linked List all seats are connected in a ring fasion so we can directly move from seat A1 to J7 using previous pointer as in previous pointer of head node address of seat J7 is stored.



------------------------------------------->Space Left for Image <---------------------------------------------------------


So lots of time gets saved which increases efficiency of the system.
FUNCTIONS USED : -
1] create() :- To create 70 nodes internally ( in memory ), each node represent one seat.Each node has 6 parameters
1) previous pointer of node* type to store address of previous node;
2) next pointer of node* type to store address of next node;
3) seat_no- to store seat number (int type)
4) row_no- to store row no(char type)
5)booking status- to show wether seat is alredy booked or available for booking(char type)
6)pin- different pin for each seat(int type)
So this function will create 70 nodes in memory locations & it will assign each node a
seat_no,booking_status and pin.
2] display() :- To display the seating arrangement ie to display the linked list.
The display will show row number followe by seat no followe by booking status (‘a’ or ‘b’ -> available/booked) of each seat/node.
“In display additional lines of codes are added to make display more powerful for LINUX TERMINAL”




------------------------------------------->Space Left for Image <---------------------------------------------------------
inux terminal output of display function



3] book_seat() :- it will take input from user as seat no. If booking status of that seat is ‘a’  then avaibility status of that seat will change from (a) to (b) . else it will show an error message. If Seat is booked succesfully the it will display pin for each seat.




------------------------------------------->Space Left for Image <---------------------------------------------------------
Linux terminal output of book_seat function



4] cancle_seat() :- the purpose of assigning pin to each seat is only one who has booked the seat can cancle it. So at the time of cancelation pins are required .
Now at cancelation time it wil ask for seat number and pin if seat number and pin combination matches and the avaibility status of that seat is booked then that seat will be cancled. Else it will give an error message.



------------------------------------------->Space Left for Image <---------------------------------------------------------
Linux terminal output of cancle_seat() function


“RUN THIS CODE IN LINUX TERMINAL FOR BETTER OUTPUT EXPIRENCE”
