USE OnlineStore;

-- Query to get all customers
SELECT * FROM Customers;

-- Query to get all products with their prices and stock quantity
SELECT ProductName, Price, StockQuantity FROM Products;

-- Query to get all orders with customer information
SELECT Orders.OrderID, Customers.FirstName, Customers.LastName, Orders.OrderDate, Orders.TotalAmount
FROM Orders
JOIN Customers ON Orders.CustomerID = Customers.CustomerID;

-- Query to get the details of a specific order
SELECT Orders.OrderID, Products.ProductName, OrderDetails.Quantity, OrderDetails.Price
FROM OrderDetails
JOIN Orders ON OrderDetails.OrderID = Orders.OrderID
JOIN Products ON OrderDetails.ProductID = Products.ProductID
WHERE Orders.OrderID = 1;
