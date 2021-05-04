- 👋 Hi, I’m @prappk
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
prappk/prappk is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

This is application for movie reservation

The flow of the application is as below

controller(TO)-->Service-->Repository(Entity)-->Model

This application can be tested through postman.
If you don't have postman,please download from
 https://www.postman.com › downloads


The following are the database tables 
USER_DB(MANUALLY CREATED)

userid(primary key)
name
age
emailid
mobnumber

THEATRE_DB(MANUALLY CREATED)

Venue
moviename
screenname
showtiming
seatnumber

BOOKINGDETAIL_DB(created through endpoints)

userid
venue
screenname
moviename
showtime
seatnumber

The endpoints are
1./MovieApp/CheckSeats
http://localhost:7001/MovieApp/CheckSeats
For checking the logic for maximum seats and same seats booking for multiple users
 

2./MovieApp/SaveBooking
For saving the user details we need to give the following json format while testing in postman

{
    "name": "pradeep1",
    "id":"userid1",
    "seatNos":"B12#B13#B14",
    "theatreId":"Theatreid2",
    "timeStamp":"05042021",
    "showTime":"134505052021"
}

3./MovieApp/Payment
For checking the payment timeout and response from payment webservice.

After successful booking, it will be inserted into booking_details_db
 









