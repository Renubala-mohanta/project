INSERT INTO Customers (customer_id, name, age, gender)
VALUES (1, 'John Doe', 25, 'Male'),
       (2, 'Jane Smith', 30, 'Female'),
       (3, 'Alex Johnson', 35, 'Male')
       
INSERT INTO Products (product_id, name, category, price)
VALUES (1, 'Product A', 'Category X', 10.99),
       (2, 'Product B', 'Category Y', 20.99),
       (3, 'Product C', 'Category Z', 15.99)
INSERT INTO Sales (transaction_id, customer_id, product_id, date, quantity, amount)
VALUES (1, 1, 1, '2023-01-01', 2, 21.98),
       (2, 2, 2, '2023-01-02', 1, 20.99),
       (3, 3, 3, '2023-01-03', 3, 47.97)

INSERT INTO Inventory (product_id, stock_count)
VALUES (1, 10),
       (2, 5),
       (3, 8)

DELETE FROM Customers WHERE customer_id IS NULL OR name IS NUll;
UPDATE Inventory SET stock_count = 0 WHERE stock_count IS NULL;


UPDATE Customers SET gender = UPPER(gender);

PRAGMA table_info(Customers);

PRAGMA table_info(Products);
PRAGMA table_info(Sales);


PRAGMA table_info(Inventory);
