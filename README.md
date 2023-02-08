# SQL

1. Напишите SQL запрос, который выведет 10 заказов, отсортированных по убыванию даты их создания (OrderDate). 
Выполнение задание было на сайте https://www.w3schools.com/sql/trysql.asp?filename=trysql_op_add

select OrderID, OrderDate, Customers.Customername from orders
join Customers ON Orders.CustomerID = Customers.CustomerID
order by OrderDate
limit 10

![Результат](https://github.com/vollmerivan/SQL/blob/main/assets/1.jpg)

2. Составьте SQL запрос:
Выбрать все категории с ИД от 2 до 7
Таблица Categories, условие фильтрации CategoryID.
(*) -  сортировка в порядке убывания .

Выполнение задание было на сайте https://www.w3schools.com/sql/trysql.asp?filename=trysql_op_add

SELECT * FROM [Categories]
where CategoryID>=2 and CategoryID<=7
order by CategoryID desc

![Результат](https://github.com/vollmerivan/SQL/blob/main/assets/2.jpg)
