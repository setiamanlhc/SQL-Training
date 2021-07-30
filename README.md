# 01. Selecting COLUMN 

##  How young are you ?
Given DOB you have to calculate the age and display the text like this "I am 40 years young"
What you learn in this exercise:
* Remark
* Define friendly column Name
* Literal or constant value
* Concate multiple values into one column
* System function current_date
* Casting and conversion

```sql
select 
date_part('year', current_date) as "Today"
, '1990-07-07'::date  as "DOB"
--, '35'::integer "Age"
, ' I am ' ||date_part('year', current_date) - date_part('year','1975-07-07'::date) || ' Years young' "Age"
;
```

## what is the number of rental days ?
In the dvdrental database you have rental table. Your task is to calculate number of rental days between rental_date and return_date.

Starting script
```sql
select * from rental limit 10
```
What you learn in this exercise.
* select all columns
* limit number of rows return
* select specific columns from table

## what are the special features in the film list?

```sql
select  special_features from film
```
What you learn in this exercise:
* using DISTINCT to eliminate duplicate rows.
*
## what is my film inventory ?
```sql
select count(1) from film
```
What you learn in this exercise?
* count rows using count function

# Filtering Rows
# Joining Tables
# Aggregate Function
