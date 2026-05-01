# SQL Practice for QA

This document contains basic SQL queries used for database testing practice.

---

## Database Structure

### Visitors Table
- Stores visitor personal data

### Rooms Table
- Contains room details and pricing

### Bookings Table
- Stores booking information and relationships between visitors and rooms

---

## Basic Queries

### Select all visitors
SELECT * FROM Visitors;

### Filter by condition
SELECT * FROM Visitors
WHERE first_name = 'John'
AND last_name = 'Smith';

### Sorting
SELECT * FROM Rooms
ORDER BY room_id;

---

## Data Manipulation

### Insert data
INSERT INTO Visitors (...)

### Update data
UPDATE Visitors
SET email = 'example@gmail.com'
WHERE visitor_id = 2;

### Delete data
DELETE FROM Visitors
WHERE visitor_id = 1;

---

## Aggregations

SELECT COUNT(*) FROM Bookings;

SELECT SUM(total_price)
FROM Bookings
WHERE status = 'Checked-in';

SELECT AVG(total_price)
FROM Bookings;

---

## Filtering

SELECT * FROM Visitors
WHERE first_name LIKE '%en%';

SELECT * FROM Rooms
WHERE price_per_night BETWEEN 800 AND 1500;

---

## Joins

### INNER JOIN
SELECT v.first_name, r.room_number
FROM Visitors v
JOIN Bookings b ON v.visitor_id = b.visitor_id
JOIN Rooms r ON b.room_id = r.room_id;

### LEFT JOIN
SELECT v.first_name, b.booking_id
FROM Visitors v
LEFT JOIN Bookings b ON v.visitor_id = b.visitor_id;