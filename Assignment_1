use bootcamp;
create table Salesman(salesman_id int primary key, name varchar(50), city varchar(50), commission varchar(50));
insert into Salesman(salesman_id,name,city,commission) values(5001,"James Hoog","New York",0.15);
insert into Salesman(salesman_id,name,city,commission) values(5002,"Nail Knite","Paris",0.13);
insert into Salesman(salesman_id,name,city,commission) values(5005,"Pit Alex","London",0.11);
insert into Salesman(salesman_id,name,city,commission) values(5006,"Mc Lyon","Paris",0.14);
insert into Salesman(salesman_id,name,city,commission) values(5007,"Paul Adam","Rome",0.13);
insert into Salesman(salesman_id,name,city,commission) values(5003,"Lauson Hen","San Jose",0.12);

select * from Salesman;

create table Customer(customer_id int, cust_name varchar(50), city varchar(50), grade int, salesman_id int, 
foreign key(salesman_id) references Salesman(salesman_id));

insert into Customer(customer_id,cust_name,city,grade,salesman_id) values(3002,"Nick Rimando","New York",100,5001);
insert into Customer(customer_id,cust_name,city,grade,salesman_id) values(3007,"Brad Davis","New York",200,5001);
insert into Customer(customer_id,cust_name,city,grade,salesman_id) values(3005,"Graham Zusi","California",200,5002);
insert into Customer(customer_id,cust_name,city,grade,salesman_id) values(3008,"Julian Green","London",300,5002);
insert into Customer(customer_id,cust_name,city,grade,salesman_id) values(3004,"Fabian Johnson","Paris",300,5006);
insert into Customer(customer_id,cust_name,city,grade,salesman_id) values(3009,"Geoff Cameron","Berlin",100,5003);
insert into Customer(customer_id,cust_name,city,grade,salesman_id) values(3003,"Jozy Altidor","Moscow",200,5007);
insert into Customer(customer_id,cust_name,city,salesman_id) values(3001,"Brad Guzan","London",5005);

select * from Customer;

select s.name as "Salesman",c.cust_name,s.city from Salesman s inner join Customer c where s.city=c.city;
  #OR
select Salesman.name as "Salesman",
Customer.cust_name, Salesman.city 
from Salesman,Customer 
where Salesman.city=Customer.city;
