# ⚡ ELECTRIFY - Electricity Billing System

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white" alt="Java Badge" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL Badge" />
  <img src="https://img.shields.io/badge/License-Academic-green?style=for-the-badge" alt="License Badge" />
</p>

## Project Overview  
ELECTRIFY is an advanced, user-friendly electricity billing management system aimed at automating and optimizing the billing process for electricity providers and consumers. It eliminates the need for manual meter reading, billing paperwork, and physical bill delivery by digitizing all operations into a secure, efficient software platform. This leads to faster processing, reduced human errors, and enhanced customer satisfaction.

---

## Key Features  
- 🔐 **Secure Role-Based Authentication:** Separate Admin and Customer logins ensure that each user sees only the data relevant to their role.  
- 🏢 **Admin Dashboard:** Enables administrators to add and manage customers, input meter readings, assign meter types, and generate bills with calculated taxes and service charges.  
- 💡 **Automated Consumption Calculation:** Calculates monthly unit consumption and total bill including penalties, ensuring accurate billing.  
- 💳 **Online Payment Integration:** Customers can conveniently pay bills through integrated payment gateways like Paytm without visiting offices.  
- 📊 **Comprehensive Reports:** Provides detailed billing histories, deposit statuses, and user information with options to print or export.  
- 🛠 **Integrated Utilities:** Includes handy tools like notepad, calculator, and web browser accessible from within the application to enhance user experience.  
- 🗄 **Robust Database:** Employs MySQL for managing customers, bills, meter info, tax, and login information with well-structured, normalized tables to maintain data integrity.  
- 🖥️ **Interactive UI:** Developed with Java Swing offering intuitive GUI components ensuring ease of use for both admins and customers.

---

## System Architecture  
- **Client-Server Desktop Application:** The system runs on a desktop environment developed using Java Swing with multi-threaded support for responsiveness.  
- **Database Layer:** MySQL serves as the backend to store and retrieve all user, billing, and meter-related data. JDBC is used to facilitate connectivity between Java application and the database.  
- **Security Measures:** Password protection, input validation, and secured queries are implemented to prevent unauthorized access and protect data.

---

## Benefits  
- 🌍 **Paperless Billing:** Eliminates physical bill generation and delivery, supporting environmental sustainability.  
- ⏱️ **Time Efficiency:** Reduces manual effort in meter reading, bill calculation, and customer interaction.  
- ✔️ **Accuracy:** Minimizes human error during calculations and data entry.  
- 🛡️ **Transparency:** Enables customers to view their consumption and billing details anytime online.  
- 💼 **User Management:** Simplifies handling of multiple users with different access privileges.

---

## Installation & Setup  
1. Ensure MySQL Server is installed and running.  
2. Import provided SQL scripts to create the required database schema and tables.  
3. Configure database connection parameters (`username`, `password`, `database URL`) in the `Conn.java` class.  
4. Import and run the project in an IDE supporting Java (NetBeans, Eclipse, etc.).  
5. Start using the application with Admin login to add customers and manage billing.

---

## Future Enhancements  
- 📁 File and Document Uploads for customers  
- 🎙️ Voice commands and support for customer service  
- 📹 Mobile app companion for remote access  
- 🔒 Enhanced security with two-factor authentication  
- 🤝 Multi-admin support with role-based controls  

---

## MySQL Queries
create database ebs;


use ebs;


create table login(meter_no varchar(20), username varchar(30), name varchar(30), password varchar(20), user varchar(20)); 


select * from login;


describe login;


create table customer(name varchar(20), meter_no varchar(20), address varchar(50), city varchar(30), state varchar(30), email varchar(40), phone varchar(20));


select*from customer


create table meter_info(meter_no varchar(20), meter_location varchar(20), meter_type varchar(20), phase_code varchar(20), bill_type varchar(20), days varchar(20));


select*from meter_info


create table tax(cost_per_unit varchar(20), meter_rent varchar(20), service_charge varchar(20), service_tax varchar(20), swacch_bharat_cess varchar(20), fixed_tax varchar(20));


insert into tax values('9','47','22','57','6','18');


select*from tax


create  table bill(meter_no varchar(20), month varchar(30), units varchar(20), totalbill varchar(20),status varchar(20));

select*from bill


drop table bill;

---


## SnapShots 

<img width="854" height="426" alt="image" src="https://github.com/user-attachments/assets/156104ae-0bd3-45b7-b855-7d3780266e6b" />

<img width="881" height="624" alt="image" src="https://github.com/user-attachments/assets/192d8d24-e9a3-4b01-b1e2-e73abb597383" />

<img width="861" height="383" alt="image" src="https://github.com/user-attachments/assets/930e48ee-8bd9-48cd-81aa-242fdab117da" />

<img width="881" height="472" alt="image" src="https://github.com/user-attachments/assets/e5a14d73-e1c2-4ccf-9413-07f4a1c0b11e" />

<img width="867" height="555" alt="image" src="https://github.com/user-attachments/assets/9a43ab2f-f7ff-4643-9339-33c69c0d5029" />

<img width="890" height="645" alt="image" src="https://github.com/user-attachments/assets/6a3f8dce-7570-4a0a-a6ab-83943aaa91e9" />

<img width="888" height="635" alt="image" src="https://github.com/user-attachments/assets/6a9a9243-06b4-44a0-8b3b-d305f2e8ab0f" />


---

## License  
This software is developed exclusively for academic project and learning purposes.

---

Made with ❤️ using Java and MySQL.

