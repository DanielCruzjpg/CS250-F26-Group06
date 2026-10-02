# BeAvis Car Rental System
Nathan Brady, Daniel Cruz,Abdul Rahim Karimi, Abdulwahab fazli, Mohammad Rasooli, Abdullah Mohammed, Mohammed Kashif...ADD NAMES HERE

## System Description
The BeAvis Car Rental System is a software platform for managing the company’s car rental operations. Customers can access it through a mobile app for iOS or Android, or through a website. Both channels allow customers to create and verify an account, sign in, find nearby rental locations, make and manage rentals, view rental history, and manage payment methods. Customers may also enable two-step authentication in their account settings.
Employees can sign in to review customer rental status and contracts, check vehicle availability, and update vehicle status when a car needs maintenance. The system supports rental agreement distribution and electronic signing, and stores signed contracts securely.
The system uses location services to help customers find nearby branches and get directions. It also integrates with email, mapping, payment, and authenticator services. Payment information and signed contracts receive restricted handling to protect sensitive customer data.

## Software Architecture Overview
### UML Use Case Diagram
<img width="473" height="356" alt="image" src="https://github.com/user-attachments/assets/bcf50f4c-b76c-4dd2-a266-7d706bc716d4" />

### UML Class Diagram:
<img width="1142" height="1540" alt="UML-Diagram drawio" src="https://github.com/user-attachments/assets/dd3df2d2-1137-4671-864e-bd3d5af260fe" />

#### Description:
This UML class diagram describes a car rental system and the main data and operations it supports.

The Users class holds shared account details and provides login, logout, and profile-update functions. Customer, Employee, and Administrator represent different user roles. Customers can search available vehicles, make or cancel reservations, and view rental history. Employees check vehicles out and in, recording details such as mileage, fuel, and damage. Administrators manage vehicles and branches and generate reports.

The system tracks its rental process through several related classes:

Branch represents a rental location and provides vehicle availability information.
Vehicle stores details such as make, model, category, mileage, daily rate, and status.
Reservation records the customer, selected vehicle, pickup and return branches, dates, status, and estimated cost.
Rental records the actual vehicle checkout and return, including mileage and fuel details.
Payment tracks charges or refunds and their status.
Invoice calculates the rental’s charges, fees, taxes, and total.
Notification represents messages such as confirmations, reminders, and receipts.
Extra represents optional add-ons with their own daily prices.
Report summarizes rental activity and revenue over a date range.
The Enumerations section lists allowed values for roles, vehicle categories and statuses, reservation and rental statuses, payment methods and statuses, and notification types. These values help keep system records consistent.

Overall, the diagram shows how customer accounts, reservations, vehicles, rentals, payments, and supporting records fit together to support the company’s rental workflow. The connection lines indicate relationships between classes; where the diagram does not show quantities, it does not specify exactly how many records can be associated.

### SWA Diagram
<img width="829" height="614" alt="Screenshot 2026-10-01 at 8 05 28 PM" src="https://github.com/user-attachments/assets/9748a0a0-64b3-4a05-a625-2ddf2eec3015" />

#### Description:

### UML Class Description:
This software architecture shows how a car rental system works. Customers use the mobile app or website, while employees use a staff portal with role-based access. Their requests go to the API/application layer, which handles login, accounts, rentals, vehicles, locations, and contracts. The system stores regular information, such as customer, employee, vehicle, and rental data, in the core data stores, while more sensitive information, such as payment references and encrypted contracts, is kept in protected storage. The security and integration layer connects the system to outside services like payment processors, email services, maps, and authenticator apps. The arrows show how information moves securely between each part of the system using HTTPS, TLS, authentication, and limited access permissions.


## Development Plan and Timeline
### 10/1/2026
#### UML Use Case Diagram
Nathan Brady, Daniel Cruz

#### UML Class Diagram
Abdullah Mohammed,
Mohammad Rasooli
Mohammed Kashif

#### SWA Diagram
Abdul Rahim Karimi 

#### SWA Description
Abdulwahab Fazli
