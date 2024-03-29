1. Создать таблицу employees
```
create table employees(
          id serial primary key,
      employee_name Varchar(50) not null
);
```
2. Наполнить таблицу employees 70 строками.
``` 
insert into employees (employee_name)
values ('Anna'), ('Olga'), ('Ola'), ('Inna'), ('Irina'), ('Ida'), ('Ira'), ('Asia'), ('Ula'), ('Sveta'),
('Kasia'), ('Kazia'), ('Beata'), ('Basia'), ('Silvia'), ('Sara'), ('Magda'), ('Maria'), ('Berta'), ('Tania'),
('Dorota'), ('Zosia'), ('Aga'), ('Fatima'), ('Gosia'), ('Lilia'), ('Luisa'), ('Lada'), ('Ludmila'), ('Lisa'),
('Lida'), ('Luba'), ('Marta'),  ('Rimma'), ('Emma'), ('Frida'),  ('Fiona'), ('Viola'), ('Fata'), ('Marina'), 
('Rosa'), ('Patricia'), ('Renata'), ('Rita'), ('Margo'), ('Alisa'), ('Ala'), ('Tara'), ('Mira'), ('Dana'),
('Missi'), ('Agata'), ('Ewa'), ('Aida'), ('Aziza'), ('Alina'), ('Dina'), ('Larisa'), ('Laura'), ('Diana'), 
('Amina'), ('Melissa'), ('Irma'), ('Marfa'), ('Iveta'), ('Ilona'),  ('Vanda'), ('Inga'), ('Bella'), ('Galina');
```
3. Создать таблицу salary
```
create table salary_1 (
      id serial primary key,
      monthly_salary int not null
);
```
4. Наполнить таблицу salary 15 строками
```
insert into salary_1 (monthly_salary)
values (1000), (1100), (1200), (1300), (1400), (1500), (1600), (1700), (1800), (1900),(2000), (2100), (2200), (2300), (2400), (2500);
```
5.Создать таблицу employee_salary
- id. Serial  primary key,
- employee_id. Int, not null, unique
- salary_id. Int, not null
```
create table employee_salary (
      id serial  primary key,
      employee_id  Int unique  not null,  
      salary_1_id  Int  not null);
```     
6. Наполнить таблицу employee_salary 40 строками:
- в 10 строк из 40 вставить несуществующие employee_id     
```     
insert into employee_salary (employee_id, salary_1_id)
values (3, 7), (1,4), (5,9), (40,13), (23,4), (11,2), (52,10), (15,13), (26,4), (16, 1),
       (37,7), (33,7), (9,15), (42, 4), (67, 8), (55, 13), (2, 16), (4, 5), (6, 10), (7, 9), 
       (8, 1), (10,11), (12, 5), (13, 15), (14, 6), (17, 7), (18, 15), (19, 7), (20, 8), (21, 3),
       (71, 4), (72,9), (73, 6), (74, 8), (75,5), (76, 13), (77, 14), (78, 16), (79, 11), (80,1);
```       
7. Создать таблицу roles
- id. Serial  primary key,
- role_name. int, not null, unique
 ```     
 create table roles_1 (
      id serial  primary key,
      role_name  Int unique  not null  
     );      
```  
8. Поменять тип столба role_name с int на varchar(30)
```    
  alter table roles_1
  alter column role_name type Varchar(30);
``` 
 9. Наполнить таблицу roles 20 строками:
 ```
 insert into roles_1 (role_name)
values ('Junior Python developer'),
('Middle Python developer'),
('Senior Python developer'),
('Junior Java developer'),
('Middle Java developer'),
('Senior Java developer'),
('Junior JavaScript developer'),
('Middle JavaScript developer'),
('Senior JavaScript developer'),
('Junior Manual QA engineer'),
('Middle Manual QA engineer'),
('Senior Manual QA engineer'),
('Project Manager'),
('Designer'),
('HR'),
('CEO'),
('Sales manager'),
('Junior Automation QA engineer'),
('Middle Automation QA engineer'),
('Senior Automation QA engineer');
```
10. Создать таблицу roles_employee
- id. Serial  primary key,
- employee_id. Int, not null, unique (внешний ключ для таблицы employees, поле id)
- role_id. Int, not null (внешний ключ для таблицы roles, поле id)
```
create table  roles_employee(
      id serial  primary key,
      employee_id Int unique  not null,
      role_id  Int not null
     );   
 ```   
11. Наполнить таблицу roles_employee 40 строками
```
insert into roles_employee (employee_id, role_id)
values (7,2), (20,4), (3,9), (5,13), (23,4), (11,2), (10,9), (22,13), (21,3), (34,4), 
       (6,7),(55,17), (37,11), (69, 6), (44,12), (45,18), (29,10), (52,5), (41,7), (39,11),
       (66,9), (50, 14), (19,19), (17,5), (31, 2), (27,17), (16,19), (60,17), (33,9), (28,11),
       (32,1), (25, 13), (4, 14), (26, 13), (47, 20),(8, 2), (9, 15), (30, 3), (12, 5), (13,20);
       
 select * from employees;
       
 select * from salary_1;

select * from employee_salary;

select * from roles_1;

select * from roles_employee;
```
