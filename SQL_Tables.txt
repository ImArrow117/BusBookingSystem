create database project;
use project;

CREATE TABLE IF NOT EXISTS register(
    id INT AUTO_INCREMENT PRIMARY KEY,
    Name VARCHAR(255) NOT NULL,
    Gender VARCHAR(255) NOT NULL,
    Email VARCHAR(255) NOT NULL,
    Password VARCHAR(255) NOT NULL
);
select* from register;
truncate table register;
truncate table booking_details;




CREATE TABLE booking_details (
	 booking_id INT AUTO_INCREMENT PRIMARY KEY,
    source VARCHAR(255) ,
    destination VARCHAR(255) ,
    date DATE ,
    bus_name varchar(255),
    bus_type VARCHAR(50) ,
    total_seats INTEGER,
    ticket_price float
);

select * from booking_details;


create table admin(
admin_id int auto_increment primary key,
username varchar(255),
password varchar(255)
);
select * from admin;
truncate table admin;

INSERT INTO admin (username, password) VALUES ('Abhijit', 'abhijit@98');
INSERT INTO admin (username, password) VALUES ('Abhishek', 'abhishek@123');
INSERT INTO admin (username, password) VALUES ('CL', 'CL@123');
INSERT INTO admin (username, password) VALUES ('Adesh', 'adesh@123');
INSERT INTO admin (username, password) VALUES ('TL', 'TL@123');
INSERT INTO admin (username, password) VALUES ('Hingmare', 'hingmare@123');
INSERT INTO admin (username, password) VALUES ('sinha', 'sinha@123');



create table buslist(
source varchar(15),
destination varchar(15),
bus_name varchar(15),
bus_type varchar(10),
total_seats int,
ticket_price float
);
drop table buslist;
truncate table buslist;
select * from buslist;

INSERT INTO buslist (source,destination,bus_name, bus_type, total_seats, ticket_price) 
VALUES 
('mumbai', 'pune','Shivshahi', 'delex', 40,250),
('mumbai', 'pune','Shivneri', 'Luxury', 40,350),
('pune', 'mumbai','Shivshai', 'AC', 42,350),
('Kolhapur', 'mumbai','MSRTC', 'Sleeper', 38,450),
('stara', 'pune','PMT', 'Delux', 45,550);