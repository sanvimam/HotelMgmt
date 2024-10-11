# HotelMgmt


# Team Name:
29704 Group 1 DearyQuery

# Team Members:
1. Sanvi Mamidipalli
2. Suhayb Ahmed
3. Neil Meza
4. Hazel Lee

# Scenario Description:
This model represents the operational structure of a resort company, focusing on managing its hotels, guest bookings, services, and staff. The system tracks how guests interact with the resort by making room reservations, using various services offered at the hotel, and making payments. It also handles the management of employees and their respective departments, ensuring smooth internal operations. Additionally, the model supports vendor relationships, where external vendors provide certain services to the guests. By using this model, the resort can effectively oversee daily activities, track guest experiences, and analyze performance across different areas such as guest satisfaction, employee management, and vendor services. The system is designed to enhance the overall management and service delivery of the resort, ensuring smooth operations across its various departments and services.

# Data Model:
This data model represents a relational structure for a resort management system. It supports the storage of various entities related to hotel operations, including hotels, rooms, guests, services, employees, vendors, payments, and invoices. Shown below is a breakdown of how data is organized and the relationships between entities.

### 1. Hotel and Room Relationship:
Each hotel can have multiple rooms associated with it. The "Hotel" entity is connected to the "Room" entity, where each room belongs to a specific hotel. This captures the relationship between a hotel's location and the rooms it manages.
### 2. Room and Reservation Relationship:
Rooms are linked to reservations. A room can be reserved through the "Reservations" entity, and the "Room_has_Reservations" table handles this many-to-many relationship, allowing multiple rooms to be part of a single reservation, and multiple reservations can be made for the same room over time.
### 3. Guests and Reservations Relationship:
Guests can make reservations for rooms, and this relationship is managed by the "Guests_has_Reservations" table, which connects the "Guests" and "Reservations" entities. This captures the information about which guest has reserved which rooms during their stay at the resort.
### 4. Services and Guests:
The model also tracks the services that guests use during their stay through the "Services_has_Guests" table. This table connects the "Services" entity with the "Guests" entity, recording what services a guest has utilized (such as dining, spa, or transportation).
### 5. Payments and Invoices:
Payments are recorded for each reservation, and these payments are linked to an invoice. The "Payments" entity connects both to the "Reservations" and the "Invoice" entities, allowing the system to track how much a guest paid for their stay and services, along with generating a corresponding invoice.
### 6. Employees and Hotel Departments:
The "Employees" entity is associated with departments within the hotel, captured by the "Department" entity. Each employee works for a department, and departments are connected to specific hotels, making it possible to track staff responsibilities and assignments within the resort.
### 7. Vendors and Services:
External vendors provide services that the resort offers. The "Vendor" entity is connected to the "Services" entity, allowing the resort to track which vendors supply which services (e.g., catering, spa treatments, transportation).

### What the Data Model Supports:
- Hotel Management: The system stores details about hotels and their rooms.
- Guest Reservations: It tracks guest information, their reservations, and the rooms they book.
- Services Usage: It supports the storage of data related to the services guests use during their stay.
- Employee Management: It tracks employee roles and department assignments within each hotel.
- Vendor and Service Tracking: It manages vendor relationships and the services provided by those vendors.
- Payment and Invoice Processing: It records payments made by guests and generates invoices related to their stays and services used.

### What the Data Model Does Not Support:
- Service Inventory: The model does not track specific inventories for services (e.g., food items for dining services or spa products).
- Customer Feedback/Surveys: There's no entity to capture guest feedback or satisfaction ratings.
- Room Cleaning and Maintenance Schedules: It does not track room cleaning or maintenance records.
- Event or Group Bookings: The model does not specifically cater to group reservations or events hosted at the resort.
- Marketing and Promotions: There's no structure for storing data related to marketing campaigns, promotions, or loyalty programs for guests.

<img width="747" alt="Screenshot 2024-10-11 at 12 41 02 PM" src="https://github.com/user-attachments/assets/d6c97aa6-b3b6-4fb9-8bbe-0da1295e14cb">

# Data Dictionary:
### Hotel Table
<img width="484" alt="Screenshot 2024-10-11 at 12 55 11 PM" src="https://github.com/user-attachments/assets/649ba87c-72df-4d37-af1c-6b9eca6d265c">

### Room Table
<img width="577" alt="Screenshot 2024-10-11 at 12 56 06 PM" src="https://github.com/user-attachments/assets/9bf0e592-50ba-43a6-a336-e3fbf6f74807">

### Reservations Table
<img width="551" alt="Screenshot 2024-10-11 at 12 56 36 PM" src="https://github.com/user-attachments/assets/7573bc84-8784-4a61-b757-461622e01c0a">

### Guests Table
<img width="482" alt="Screenshot 2024-10-11 at 12 57 15 PM" src="https://github.com/user-attachments/assets/f686d3c8-bb22-42c0-bdad-4d63268b582e">

### Payments Table
<img width="544" alt="Screenshot 2024-10-11 at 12 57 42 PM" src="https://github.com/user-attachments/assets/edc09994-f3d0-49cd-bba0-09ae9937b6be">

### Services Table
<img width="521" alt="Screenshot 2024-10-11 at 12 58 21 PM" src="https://github.com/user-attachments/assets/60bc3c8f-b693-449b-8485-7d8822e77bcf">

### Employees Table
<img width="559" alt="Screenshot 2024-10-11 at 12 59 07 PM" src="https://github.com/user-attachments/assets/63c728c6-5b19-439f-bad1-95d2be883605">

### Department Table
<img width="522" alt="Screenshot 2024-10-11 at 12 59 42 PM" src="https://github.com/user-attachments/assets/c14774b6-23d5-4b9a-9600-a829d690a4c4">

### Vendor Table
<img width="497" alt="Screenshot 2024-10-11 at 1 00 10 PM" src="https://github.com/user-attachments/assets/3b953941-df7a-49e4-9284-a10859aa8990">

### Invoice Table
<img width="494" alt="Screenshot 2024-10-11 at 1 00 34 PM" src="https://github.com/user-attachments/assets/6f288e37-c941-4359-a30e-9496bd4e89ea">

# Queries:










