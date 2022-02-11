# DBMS-PRORAM
create table student(name varchar(20),roll int);
insert into student values('RAM',4);
update student set name = 'Ritu' where roll = 65;
alter table student add id int;
delete from student where name = 'Ritu';
select *from student;


select *from student where name ='Ritu',and roll=65;
select *from student where name ='Ritu' or name='Devarsha';
select *from student where not name ='Ritu';
select *from student where roll between 8 and 65;
select *from student where name like '%a';

select min (price) as smallest price from products;
select max (price) as largest price from products;
select count (price) from products;
select avg (price) from products;
select sum (price) from products;

select name ,city from student where address is null;

create table product(personid  not null primary key name varchar(255) not null);
create table product(person id int not null primary key order number int not null person id int  foreign key reference person(person id);

alter table table name 
add primary key(columnname);

alter table tablename 
add constraintname
foreign(columnname)reference tablename;

alter table tablename 
drop primry key
drop primary key;

alter table table name 
drop constaint constraintname;

select column_name(s)
from table_name
where condition
group by column_name(s)
order by column_name(s);

select count(customerid) country;
from customers
group by country;

select column_name(s) from table1;
union all
select column_name(s) from table2
