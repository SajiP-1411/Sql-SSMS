create database task;

--create a table--

create table employee_data(FirstName varchar(10),LastName varchar(10),DOB int,MaritalStatus	varchar(10),Gender varchar(10),EmailAddress varchar(50),AnnualIncome int,Occupation varchar(40)
);

select * from employee_data

insert into employee_data values('john','smith',2003,'single','M','johnsmith@gmail.com',50000,'Software Engineer')
insert into employee_data values('celine','peter',2000,'married','F','celinepeter@gmail.com',75000,'Business Analyst')
insert into employee_data values('uma','maheswari',1998,'married','F','maheswari323@gmail.com',55000,'Asst Professor')
insert into employee_data values('sam','daniel',2000,'married','M','samdan@gmail.com',40000,'PED Teacher')
insert into employee_data values('raj','kumar',2002,'single','M','raj65@gmail.com',55000,'Web Developer')
insert into employee_data values('sri','krishnan',1995,'married','M','krishnan@gmail.com',45000,'Civil Engineer')
insert into employee_data values('nithya','ram',1998,'married','F','nithya24@gmail.com',65000,'Doctor')
insert into employee_data values('pranav','dith',2000,'single','M','pranav@gmail.com',50000,'Software Engineer')
insert into employee_data values('ragul','mahesh',1996,'married','M','rahul@gmail.com',50000,'Teacher')
insert into employee_data values('priya','bhat',2000,'single','F','priya23@gmail.com',45000,'Senior Associate')


--retrieve all columns from the table you have created--

select * from employee_data

--retrieve any two columns from the table you have craeted--

select firstname,occupation from employee_data

--filter the columns by comparing the values--

select firstname,Occupation from employee_data where  "occupation" ='Software Engineer'

--filter the table and retrieve the next value--

select Occupation from employee_data order by difference (occupation,'softwareengineer')DESC

--filter and find some exact value--

select min(EmailAddress) from employee_data where EmailAddress >'priya'