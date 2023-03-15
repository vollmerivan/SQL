# SQL

 Таблицы, с которыми предстоит работать:: заказы (Orders) и клиенты (Customers), найти их можно тут:
https://www.w3schools.com/sql/trysql.asp?filename=trysql_asc

Необходимо вывести id клиента и имя клиента, сделавших больше 5-ти заказов, а также количество заказов и дату последнего заказа. Список должен идти по убыванию от  клиентов с большим количеством заказов к клиентам с меньшим количеством заказов

SELECT Customers.CustomerID, Customers.CustomerName, orders.OrderDate, COUNT (CustomerName) as kolichestvoZakazov FROM [Customers]
JOIN Orders ON Orders.CustomerID = Customers.CustomerID
GROUP BY CustomerName
HAVING kolichestvoZakazov >= 6
order by kolichestvoZakazov DESC

![image](https://user-images.githubusercontent.com/108756609/225240317-66342c7e-b05f-4e61-9008-64a842f3e13f.png)
