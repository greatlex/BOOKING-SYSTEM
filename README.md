# BOOKING-SYSTE<!DOCTYPE html>
<html>
<body>

<h2>Book an Appointment</h2>

<form action="{% url 'booking:create' %}" method="post">
  {% csrf_token %}
  <label for="customer_name">Customer Name:</label>
  <input type="text" id="customer_name" name="customer_name"><br><br>
  <label for="date">Date:</label>
  <input type="date" id="date" name="date"><br><br>
  <label for="time">Time:</label>
  <input type="time" id="time" name="time"><br><br>
  <input type="submit" value="Book Appointment">
</form>

</body>
</html>
