- SELECT name
FROM waiters
WHERE restaurant = 'Bengaluru South' AND age BETWEEN 20 AND 30
SELECT DISTINCT c.address
FROM customers c
JOIN orders o ON c.customer_id = o.customer_id
JOIN waiters w ON o.waiter_id = w.waiter_id
JOIN restaurants r ON w.restaurant_id = r.restaurant_id
WHERE r.name = 'Bengaluru South' AND w.age BETWEEN 20 AND 30;
