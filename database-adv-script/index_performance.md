### Objective 1: Identify high-usage columns in your User, Booking, and Property tables (e.g., columns used in WHERE, JOIN, ORDER BY clauses).
- Users:
	- user_id: Used in joins with Bookings (e.g., Bookings.user_id = Users.user_id) and filtering user-specific data.
- Bookings:
	- user_id: Used in joins with Users and filtering bookings by user.
	- property_id: Used in joins with Properties and filtering bookings by property.
	- start_date: Used in WHERE clauses for date range queries (e.g., start_date >= '2025-01-01').
- Properties:
	- property_id: Used in joins with Bookings and Reviews.
	- location: Used in WHERE or GROUP BY clauses for location-based filtering (e.g., location = 'New York').
	- host_id: Used in joins with Users to find properties by host.
