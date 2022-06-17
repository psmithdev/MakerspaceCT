# MakerspaceCT
## Online Machine and Tool Reservation System

MakerspaceCT
Address/Website:
960 Main Street, Hartford, CT 06103
https://makerspacect.com/
Points of Contact:
Mark Colbert
Ben Parker

## Problems and Solutions
<em>Background:</em>
MakerspaceCT shares a common problem with most shops out there: the machines and tools sit idle most of the time. The shop owners invested a ton of money to purchase assets, and they are underutilized. A machine that does not run is wasting time and money.  
MakerspaceCT wants to create their own systems internally to allow members easy access to these machines and tools–to reduce the amount of friction in getting it into their hands.
MakerspaceCT is a nonprofit shop focused on education and classes for their members. Education provides a potential career path in manufacturing for youngsters.

## Online Machine and tool Reservation System
Problem: Member comes in to use a specific/niche machine and another member is currently using it.  The machine could be in use for 2 hours or more.
Woodshop: Wood lathe.  Techno CNC router
Electronics lab: Red 60W Laser Engraver
Machine shop: Haas CNC milling machine
Metal shop: Koike Aronson ShopPro Plasma Cutting CNC
Solution: Create a reservation system that allows a member to use the current MakerspaceCT website to pick a time slot
Allow small tools as a rental outside of the shop for member.  Say dewalt drill/driver or a grinder.  Member sign liability forms for risk, and use the reservation system to rent out the tool for use.
Piece of Hardware or screen present at the machine to show time slots currently taken, so any member will know who is currently running the machine.  A piece of paper printed at the start of the day could be a temporary setup, but a waste of paper over time.  A list of names at the start of the day of members who want to use the machine.

David, shop manager, wants a POS system for selling consumables.
Problem:  Member forgets to bring in their own consumables when using a sanding tool in the metal or wood shop, or anything else.  Borrows some of the sandpaper at the shop expense, not sustainable.
Solution: P.O.S. point of sale register.  Think of a coffee shop using an iPad square device to collect payment or donation.  Direct member to MakerspaceCT website with QR code on consumable wall in the shop.
Consumables
Woodshop: sandpaper, glue, steel wool, rags
Metal shop: sanding discs for grinders, filler wire welding
Machine shop: bits

Ben, instructor, text students with Wild Apricot software
Problem: used a service called ZipWhip to text a scheduled message to  students with MakerspaceCT phone number when class is in session.  The service will reach end-of-life this year.
Solution: Integrate group text message capabilities with current Wild Apricot software using MakerspaceCT phone number
Research was performed on what are the alternatives and Integromat/Make is a service that may do the job, but requires a yearly subscription.


## Specific Needs
When a user does THAT, THIS happens.
Write out as many of these user stories to determine exactly which functionalities need to be built and find out what the exact needs of the reservation system are.
First
Second
Third

### Solutions:
OPTION 1
Use existing plugins with no modifications. You can use any that is being actively maintained.
PROS:
Get them up and running the quickest
Minimum amount of maintenance and work
CONS:
Potential security vulnerabilities
Might not meet needs
Least amount of flexibility

OPTION 2
Use the existing open-source reservation system. We can use any Wordpress plugin that we have permission to modify and use.
PROS:
Work involved to modify it (minor)
Maintenance involved (minor)
CONS:



OPTION 3
Build new system entirely
PROS:
More control
Data collection that allows for better decision making
CONS:
The most amount of work
Maintenance involved (major)
Responsible for security vulnerabilities


User Stories
(Note–we should also include stories for those who administer and moderate the system.)

PURPLE
WEB-APP USE
As a user, I can log into the web app to manage my reservations at MakerspaceCT.

SYSTEM
As the system, I send an email confirmation to the user when a reservation is made.
As the system, I block off the date/time of a reservation to prevent other members from making a reservation for the same time.
When a reservation is added to the calendar, the time slot for the reservation is blocked off for anybody else to make a reservation during that time.

# [CRUD = Create, Read, Update, and Delete]

C – ADD NEW RESERVATION
As a user, I can Add a reservation [for a machine] to the Calendar from the dedicated Reservations page.
When the user accesses the website logged in and browses to the reservation page, the reservation calendar appears with add, edit and delete functionality.
As a user, while Adding, I can configure the details [tbd] of my new reservation.
When a user clicks the Add button, a form pops up that gives them options to provide specific details about their reservation.
As a user, I receive a confirmation email for the new reservation.

R – VIEW RESERVATIONS
As a user, I can see my reservations on the calendar.
When a user selects the details about their reservation and clicks “add”, their reservation is added to the calendar.
NEW: As a user, I can see what days/times are available for [selected equipment] without attempting to create a reservation.

U – EDIT RESERVATION
As a user, I can Edit the details of my Reservation(s).
When a user chooses to edit their reservation, the form will pop up for them to make edits.
As a user, I am able to quickly Edit a Reservation by following a hyperlink in its confirmation email.

D – CANCEL RESERVATION
As a user, I can Cancel any of my (upcoming +/- ongoing?) Reservations.
As a user, I am able to quickly Cancel a Reservation by following a hyperlink in its confirmation email.

## INFORMATION
As a user, I am able to reference MakerspaceCT’s reservation rules from the Reservation Calendar page.
When a user browses to the screen with the reservation calendar, there is a list of reservation rules to ensure users are using the reservation calendar properly. (reservation maximum, no-show policy, etc)

GREEN
ADDING
As a user, I can add, edit, or delete my reservations from the calendar on a dedicated page.
When the user logs onto the website logged in and browses to the reservation page, the reservation calendar appears with add, edit and delete functionality.
As a user, I can configure certain details [tbd] when Adding a new reservation.
When a user clicks the Add button, a form pops up that gives them options to provide specific details about their reservation.
As a user, I can see my reservations on the calendar.
When a user selects the details about their reservation and clicks “add”, their reservation is added to the calendar.
As the system, I block off the date/time of a reservation to prevent other members from making a reservation for the same time.
When a reservation is added to the calendar, the time slot for the reservation is blocked off for anybody else to make a reservation during that time.
As the system, I send an email confirmation to the user when a reservation is made.
As a user, I can [manage] my reservation by following hyperlink(s) in the confirmation email.
When a reservation is added to the calendar, the user receives an email with a reservation confirmation and options to edit or delete their reservation.

EDITING
As a user, I can Edit the details of my reservation on the web app.
When a user chooses to edit their reservation, the form will pop up for them to make edits.

DELETING
As the system, I remove Canceled reservations from the Reservation Calendar
When a user chooses to delete/cancel a reservation, that reservation is deleted from the reservation calendar.
INFORMATION
As a user, I am able to quickly reference MakerspaceCT’s reservation rules from the Reservation Calendar page.
When a user browses to the screen with the reservation calendar, there is a list of reservation rules to ensure users are using the reservation calendar properly. (reservation maximum, no-show policy, etc)



Glossary: Member, Machine, Tool
Edge Cases
Scenario One
    Member Joe wants to reserve a machine or tool at MakerspaceCT.  He uses his smartphone to login to the MakerspaceCT website.  He is presented with a calendar.  He can pick a day and time that works for him during shop operating hours.  Example Sunday 12pm-2pm. Member Joe does this a few days in advance.  Shop tech employee will print out a list of machines or tools reserved that day.

Scenario Two
    Member Alyssa calls the shop to reserve a machine or tool.  The shop tech takes the call, and uses the MakerspaceCT website to make a reservation.

Scenario Three
    Member Bobby wants to reserve a tool the same day.
Scenario Four
    Member wants to reserve 2 months from now, out of town.  Coming from New York.
Scenario Five
    Member makes a reservation.  No call no show.  What is the penalty?
Scenario Six
    Member does not have access to his smartphone.  A shop tech is busy assisting another member in the shop.  There are several public computers in the shop.
Scenario Seven
    Member makes a maximum reservation time of 3 hours for the machine, only uses 1 hour.
Scenario Eight


#### Appendix 1: Bigger Picture 

The notes are a condensed representation of the areas of improvement for MakerspaceCT, as identified by Mark during the initial meeting with O(1) on Sunday, May 29th.

The 3 MakerspaceCT needs are: 
IT, Facility, Community
IT
Server System In-House
operations, upgrades, repairs, licensing, etc.
in-house networked computers
Web App/Software
reservation system(see above sections)
POS / payment system
text alerts (to high school students)
replacing Zipwhip, which is closing
Facility
access control
show certs/credentials/clearances
show additional information for members walking in
protect system
current members’ information
against vindictive ex-members (revoke access)
physical server and network monitoring and maintenance

Community
…
Appendix 2: misc notes

Problem statement: 
documentation of a problem or opportunity for improvement
a starting point for change proposals
problem statements aren't requirements or solution designs. 
they state a problem–without making assumptions about solutions
