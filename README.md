# airbnb-clone-project

<h3> project goals</h3>

<p>The backend for the Airbnb Clone project is designed to provide a robust and scalable foundation for managing user interactions, property listings, bookings, and payments. This backend will support various functionalities required to mimic the core features of Airbnb, ensuring a smooth experience for users and hosts.</p>

<h3> Technology Stack</h3>

<b>Django</b>: A high-level Python web framework used for building the RESTful API.
</br><b>Django REST Framework</b>: Provides tools for creating and managing RESTful APIs.
</br><b>PostgreSQL</b>: A powerful relational database used for data storage.

</br><b>GraphQL</b>: Allows for flexible and efficient querying of data.
</br><b>Celery</b>: For handling asynchronous tasks such as sending notifications or processing payments.
</br><b>Redis</b>: Used for caching and session management.
</br><b>Docker</b>: Containerization tool for consistent development and deployment environments.</br>
<b>CI/CD Pipelines</b>: Automated pipelines for testing and deploying code changes.


<h3> 👥 Team Roles</h3>
</br><b>Backend Developer</b>: Responsible for implementing API endpoints, database schemas, and business logic.
</br><b>Database Administrator</b>: Manages database design, indexing, and optimizations.
</br><b>DevOps Engineer</b>: Handles deployment, monitoring, and scaling of the backend services.
</br><b>QA Engineer</b>: Ensures the backend functionalities are thoroughly tested and meet quality standards.

<h3>Database Design:
key entities</h3>

</br><b>Users</b>: name - username - password - gmail ( the user can have multiple properties)- (the user can book multiple time)
</br><b>Properties</b>: image - name - price - area - user_id (properties belongs to only one user at a time) (properties can have multiple reviews )
</br><b>Bookings</b>: id - user_id - property_id - tart_date- end_date- status  (the booking belongs to one user and one propertie)
</br><b>Payments</b>: total payment - discount - amount - booking_id (the payment belongs to one booking)
</br><b>Reviews</b>: message - star_rate - property_id - user_id  (the review belongs to propertie and user)

<h5>Relations (ERD style)</h5>
 </br><b>User (1) —— (∞) Property
 </br>User (1) —— (∞) Booking
 </br>Property (1) —— (∞) Booking
 </br>Booking (1) —— (1) Payment
 </br>Property (1) —— (∞) Review
 </br>User (1) —— (∞) Review </b>

