# Group 8 MIST 4610 Project 1

# Team Name:
29704 Group 8

# Team Members:
1. Clara Wilt [@clarawilt](https://github.com/clarawilt)
2. Jaelin Cummings [@jcummings1](https://github.com/jcummings1)
3. Colby Fielding [@cpf40265](https://github.com/cpf40265)
4. Backam Nguyen [@bn51725](https://github.com/bn51725)
5. Aiman Lalani [@aal96125](https://github.com/aal96125)

# Problem Description:
The client scenario we are modeling revolves around the operations of Elite Tennis Academy. The client’s primary goal is to optimize club operations as the Elite Tennis Academy offers a variety of tennis-related services and programs that cater to a diverse clientele. The services include coaching, membership options, court reservations, tournament hosting, and various club events. Clients can utilize the online booking system to streamline the services offered. The mission of Elite Tennis Academy is to utilize the model and database to create structured queries to provide insight into the Tennis Elite Academy and resources it has to offer.


# Data Model:
Data Model:  
Our model represents the Tennis Elite Academy located in Atlanta, Georgia. The model begins with the Member entity, which holds information about the club’s members, including their unique member IDs, names, contact information, membership type, and member affiliated fees. The members can have multiple Coaches, which include their unique ID, their name, years of experience, salary, and point of contact, and the coaches can have multiple members providing a many-to-many relationship through Practices. The practices have unique IDs, dates, and durations of practice length by hours. Many practices can happen on one Court, but only one court is associated with a single practice. The court has attributes consisting of a unique court ID, court number, and court capacity. 

The Events that take place in Elite Tennis Academy have a unique event ID, event name, event date, and event themes (Graduation, Birthday, Retirement, Corporate Events, and Reunions). One Patron can have many bookings, but one booking belongs to one patron. Patrons have attributes containing a unique ID, patron name, and contact information (Phone and Email Address). One court can have many Bookings, consisting of a unique booking ID, date, and fee associated with the booking but one booking belongs to one court. The Elite Tennis Academy has many GroundKeepers that maintain the courts and are identified by a unique ID, full name, years of experience, salary, and point of contact, explaining the many-to-many relationship between courts and groundkeepers, connected by the Maintenance associative table. The maintenance table consists of the maintenance description and the date of maintenance. 

The Elite Tennis Academy hosts many Tournaments which have attributes of tournament ID, name of tournament, date and the number of players in the tournament. Tournaments have many Guests, which consists of their unique ID, the guest’s name, and their type (Adolescent, Adult, Senior) that Attend. The academy consists of multiple Courts which have a unique court ID, their court number, and the capacity it holds. Within the courts are Players (with a unique player ID, their name, their age, and their rank) that participate in Matches that show an many-to-many relationship between players and courts.


<img width="716" alt="Screenshot 2023-11-03 at 11 20 08 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/4c0bb67a-67f3-4406-a643-5395670f69c4">


# Data Dictionary: 
<img width="643" alt="Screenshot 2023-11-03 at 11 22 10 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/69cb816f-1350-4359-bbbb-33049647b229">

<img width="581" alt="Screenshot 2023-11-03 at 11 38 53 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/e1e7e7a3-a729-49a0-bb3a-8348625e4f38">

<img width="589" alt="Screenshot 2023-11-03 at 11 39 23 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/358b57fa-dc32-48e8-b277-11bc65f8f2b2">

<img width="635" alt="Screenshot 2023-11-03 at 11 25 22 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/c44d10fb-889e-44ed-8758-fb59839903e1">

<img width="590" alt="Screenshot 2023-11-03 at 11 41 31 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/bdbb459c-4162-4cf1-9491-d4cee768c5dd">

<img width="574" alt="Screenshot 2023-11-03 at 11 37 40 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/e4d9fe97-7c8e-4ab5-af2d-aa26ea2b2215">

<img width="575" alt="Screenshot 2023-11-03 at 11 38 18 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/559bb1a3-12f2-4ca8-8b89-390fc2288d0d">

<img width="493" alt="Screenshot 2023-11-03 at 11 42 31 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/fd4e3873-b097-4b43-ba0b-0376c264d296">


<img width="490" alt="Screenshot 2023-11-03 at 11 43 13 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/e7dd4ad6-0fc5-4afa-bac2-87025a0682f7">

<img width="489" alt="Screenshot 2023-11-03 at 11 43 41 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/37c1f30d-eb6e-4828-b889-e428a9fae539">

<img width="498" alt="Screenshot 2023-11-03 at 11 44 54 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/7fcd245b-3636-4a00-8aba-07cd1a156cb1">

<img width="510" alt="Screenshot 2023-11-03 at 11 45 14 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/4fc376eb-8dda-426a-b5bc-44ff55ff25be">

<img width="327" alt="Screenshot 2023-11-03 at 11 46 49 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/da5d3723-5f2d-4dc8-ad7f-a68b341ea025">

<img width="578" alt="Screenshot 2023-11-03 at 11 47 13 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/868e5ee7-89f7-489f-923f-2ac219fe3885">


# Queries:
<img width="691" alt="Screenshot 2023-11-03 at 11 49 09 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/6c282913-c752-4958-ba1a-f11b7b4f3b1c">



1. Query 1 lists the coach name, years of experience, and salary ordered by descending years of experience.
<img width="626" alt="Screenshot 2023-11-03 at 10 19 42 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/0d7fd690-13e0-4814-926a-c76102215fb0">

Query 1 allows managers to get a good general overview of each coach. Coach salary and years of experience can be essential data points used for         contract negotiations and renewals. It can help both managers and coaches ensure that the terms of the contract are fair and competitive.

2. Query 2 lists the groundkeepers who has the most maintenance jobs.
<img width="716" alt="Screenshot 2023-11-03 at 11 51 18 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/89f2654c-b91b-41ef-aedb-ed0cd438c862">

Query 2 allows managers to see which groundkeeper has the highest workload. They are then able to consider this groundkeeper for a pay raise or lighten their workload and make it equal between all groundkeepers. 

4. Query 3 lists the court number and its capacity if the capacity is greater than or equal to 200 and less than 400. 
<img width="620" alt="Screenshot 2023-11-03 at 10 44 49 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/abd359f4-8a4f-43cc-8136-3d8708457a55">

Query 3 is useful because the court capacities determine how many spectators can be accommodated in each stadium or court. This information is crucial for ticket sales and pricing, seating arrangements, and scheduling and match coordination when planning out matches with medium anticipated attendance. 

4. Query 4 shows the member type and the number of members in each type.
<img width="614" alt="Screenshot 2023-11-03 at 11 15 44 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/f2876454-8a70-4eb7-b8d3-da7550fb5402">

Query 4 is useful because the management of the tennis club will need to keep a running tally of each type to maintain their ideal membership total.

5. Query 5 lists the average booking fee among all birthday themed events.
<img width="623" alt="Screenshot 2023-11-03 at 10 29 11 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/3be97486-001c-4617-b67c-d5111ec2ccc5">

Query 5 allows managers to create a baseline estimate for customers inquiring about hosting possible birthday events. This allows the process of booking a birthday even to be streamlined and more efficient for both parties.

6. Query 6 shows the percentage of adolescent guests that attended the tournaments throughout the calendar year.
<img width="621" alt="Screenshot 2023-11-03 at 10 30 19 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/789ac5c1-5002-4b34-a5a0-91f3aa5e60e4">

Query 6 is useful for managers because it shows the distribution of adolescents at the tournaments. With this figure managers can determine whether or not they want to attempt to maintain this number or market towards increasing it for the coming year.

7. Query 7 lists the name and salary of the highest paid coach
<img width="371" alt="Screenshot 2023-11-03 at 10 31 07 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/86777db5-8237-4fe5-8c22-d5ce419f61c9">

Query 7 is useful because the salry of the highest paid coach is crucial for making strategic decisions regarding the composition and structure of the coaching staff. It can influence decisions about promoting, hiring, or reassigning coaches to align with the organization's goals.

8. Query 8 lists the total booking fees for each court, and lists these in descending order.
<img width="621" alt="Screenshot 2023-11-03 at 10 32 13 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/fe527e04-ec27-4870-a0af-1b5482ab3f78">

Query 8 is useful because it analyzes which courts generate the most revenue and then managers can tailor marketing and promotion efforts to highlight those specific courts, attracting more customers and increasing overall bookings. Courts with the most revenue can be given peak time slots to maximize profits and engagement. 

9. Query 9 lists out the player’s information for those whose age is greater than the average age of all players. It is ordered from the oldest age to the youngest age.
<img width="613" alt="Screenshot 2023-11-03 at 10 39 06 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/eb9776e9-cbc6-49c0-8f7f-a3a8bbf74d41">

Query 9 can be useful for program development. Different age groups can influence the types of activities and programs these players may want to participate in. The tennis club can then tailor its advertising promotions to specific age groups. 

10. Query 10 shows the names of patrons who have not yet booked an event.
<img width="601" alt="Screenshot 2023-11-03 at 10 56 04 AM" src="https://github.com/clarawilt/Group8MIST4610Project1/assets/131196224/7840e495-2b66-4967-b7a1-0690fdead5e1">

Query 10 would be useful information for management because they can reach out to these patrons via email or phone. By reaching out to them, they can understand their reasons for not booking an event and address any concerns the patron may have. 


# Database Information:
Name of the database: ns_F2329704Group8

Additional information: Each query listed above is marked in the database using stored procedures which can be called by using the following format: 
CALL TP_Qx where x is the number of the query.
