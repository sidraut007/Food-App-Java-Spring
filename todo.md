-- Insert data into meal table
INSERT INTO meal (name, description, price, is_deleted, meal_type_id)
VALUES 
('Pancakes', 'Fluffy pancakes with syrup', 200, b'0', 1),  -- Breakfast
('Burger', 'Grilled chicken burger with cheese', 300, b'0', 2),  -- Lunch
('Salad', 'Fresh vegetable salad', 150, b'0', 3);  -- Dinner




-- Insert data into meal_type
INSERT INTO meal_type (type_name, description, is_deleted)
VALUES 
('Breakfast', 'Morning meals like pancakes and eggs', b'0'),
('Lunch', 'Mid-day meals like burgers and pasta', b'0'),
('Dinner', 'Evening meals like salads and steaks', b'0');
