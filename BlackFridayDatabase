create database black_friday_db;
use black_friday_db;

create table incidents(
store varchar (200),
place varchar(200), 
deaths int,
injuries int,
cause varchar(200),
year int
)
;

create table deals(
store varchar (200),
category varchar(200),
offer varchar(200),
description varchar(2000),
year int
)
;



select concat('store', 'year');
SELECT CONCAT(deals.store, ',', deals.year) AS storeyear,
       deals.*
FROM   `deals`;


INSERT INTO `incidents_final`
SELECT 
store,
place, 
deaths,
injuries,
cause,
CONCAT(incidents.store, ',', incidents.year) AS storeyear,
year
FROM   `incidents`;

INSERT INTO `deals_final`
SELECT 
store,
category, 
offer,
description,
CONCAT(deals.store, ',', deals.year) AS storeyear,
year
FROM   `deals`;

create table incidents_Final(
store varchar (200),
place varchar(200), 
deaths int,
injuries int,
cause varchar(200),
storeyear varchar(50),
year int
);

create table deals_final(
store varchar (200),
category varchar(200),
offer varchar(200),
description varchar(2000),
storeyear varchar(50),
year int
)
;
 select * from deals_final;
 drop table deals;
 drop table incidents;
alter table deals_final add primary key (storeyear);
