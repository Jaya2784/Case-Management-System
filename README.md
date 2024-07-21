# LegalCase-Management-System
The proposed Database Management System (DBMS) for legal case management is an invaluable tool designed to centralize and enhance the utility of legal data. Utilizing a relational database structure, it ensures seamless integration and retrieval of information, promoting data consistency and accuracy while reducing discrepancies in legal records. The interlinked tables offer a holistic view of case information, enabling legal teams to draw meaningful correlations between client history, court proceedings, and attorney details. 

This approach streamlines workflows and fosters a collaborative environment where real-time data sharing leads to more informed and strategic decision-making. With a simple user interface, the DBMS enhances accessibility and security of case-related information, ultimately contributing to more successful legal outcomes.

# ER DIAGRAM

![image](https://github.com/user-attachments/assets/7e6b394b-d4d2-4811-99c0-84aa3bdf186a)

# SCHEMA

1. client files(client_id , first_name ,last_name) 
2. clientnew(client_id ,contact ) 
3. attorney(attorney_id,first_name ,last_name ,assigned_cases,client_id) 
4. attorneynew(attorney_id,contact) 
5. worksfor(client_id , attorney_id) 
6. court(court_id, location ,assigned_judges ,name) 
7. case conductedin(case_id ,court_id ,client_id,attorney_id ,title) 
8. casenew(case_id,hearning_dates) 
9. hearing includes(log_id, case_id ,court_id) 
10. evidence presentedwith(evidence_id, description ,photo,video ,date_obtained ,case_id) 
11. documents submittedwith(doc_id , case_id ,contents ,evidence_id) 
12. can_alsobe(doc_id ,evidence_id)  
13. appeal on(appeal_id , case_id ,status) 
14. grounds on(id, terms, appeal_id) 
15. verdict leadsto(settlement ,settlement_details ,verdict_date ,log_id) 

# FRONTEND

The program features a login window for users to enter their credentials, leading to a data 
entry window upon successful login. This window facilitates the input of various legal case 
details, submitted to a MySQL database. GUI components are styled using tkinter for a modern 
appearance. The application allows for efficient management of legal case information.

USER AUTHENTICATION PAGE

![image](https://github.com/user-attachments/assets/9cfcdcfa-0367-4cf0-b96f-5f6aebc02f71)

DATA ENTRY PAGE

![image](https://github.com/user-attachments/assets/ba5a9b21-b86d-4ec2-9102-5b1fc99e7f11)
