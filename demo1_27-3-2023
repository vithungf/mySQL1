create database saleManager;

use saleManager;

create table Product(
id_Product int not null primary key auto_increment,
nameProduct varchar(255) not null,
idCatagory int not null,
foreign key (idCatagory) references catagory(idCatagory),
price int not null default 0,
quantity int not null default 0,
discription varchar(255) null

);

create table catagory(
idCatagory int not null primary key auto_increment,
nameCatagory varchar(100) not null
);

create table customer(
idCustomer int not null primary key auto_increment,
nameCustomer varchar(255) not null,
age int not null,
phoneNumber varchar(10) not null,
address varchar(255) null
);

create table bill(
idBill int not null primary key auto_increment,
timebye datetime,
totalMoney int not null,
idCustomer int not null,
foreign key (idCustomer) references customer(idCustomer)
);

create table Productbill(
id_Product int not null,
foreign key (id_Product) references product(id_Product),
idBill int not null,
foreign key (idBill) references bill(idBill)
);
