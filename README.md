# M-K-Bounce-House
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>M&K Bouncy Houses</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      background-color: #f7f7f7;
      color: #333;
    }

    header {
      background: linear-gradient(to right, #6dd5ed, #2193b0);
      color: white;
      padding: 20px;
      text-align: center;
    }

    nav {
      background-color: #fff;
      padding: 10px;
      text-align: center;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }

    nav a {
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
      color: #2193b0;
    }

    section {
      padding: 30px;
    }

    .form-container {
      background-color: white;
      padding: 20px;
      border-radius: 8px;
      max-width: 600px;
      margin: auto;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    .form-container h2 {
      text-align: center;
    }

    .form-group {
      margin-bottom: 15px;
    }

    .form-group label {
      display: block;
      font-weight: bold;
      margin-bottom: 5px;
    }

    .form-group input,
    .form-group select {
      width: 100%;
      padding: 10px;
      border-radius: 5px;
      border: 1px solid #ccc;
    }

    button {
      background-color: #28a745;
      color: white;
      padding: 12px 20px;
      border: none;
      border-radius: 5px;
      font-size: 16px;
      cursor: pointer;
      width: 100%;
    }

    button:hover {
      background-color: #218838;
    }

    footer {
      text-align: center;
      padding: 15px;
      background-color: #2193b0;
      color: white;
    }

    .calendar-placeholder {
      text-align: center;
      margin-bottom: 20px;
      font-style: italic;
      color: gray;
    }
  </style>
</head>
<body>

  <header>
    <h1>M&K Bouncy Houses</h1>
    <p>Fun for the whole family — Serving Bristol, MA (Weekends Only)</p>
  </header>

  <nav>
    <a href="#booking">Book Now</a>
    <a href="#contact">Contact</a>
    <a href="#info">Rental Info</a>
  </nav>

  <section id="booking">
    <div class="form-container">
      <h2>Book Your Bouncy House</h2>

      <div class="calendar-placeholder">
        📅 Calendar Integration Coming Soon (weekends only, Bristol MA)
      </div>

      <form id="bookingForm">
        <div class="form-group">
          <label for="name">Full Name</label>
          <input type="text" id="name" name="name" required />
        </div>

        <div class="form-group">
          <label for="date">Rental Date</label>
          <input type="date" id="date" name="date" required />
        </div>

        <div class="form-group">
          <label for="time">Drop-Off Time</label>
          <input type="time" id="time" name="time" required />
        </div>

        <div class="form-group">
          <label for="phone">Call Back Number</label>
          <input type="tel" id="phone" name="phone" required />
        </div>

        <div class="form-group">
          <label for="house">Choose Bouncy House</label>
          <select id="house" name="house" required>
            <option value="">--Select One--</option>
            <option value="castle">Castle Themed</option>
            <option value="jungle">Jungle Themed</option>
          </select>
        </div>

        <div class="form-group">
          <label>
            <input type="checkbox" name="overnight" /> Request Overnight Rental
          </label>
        </div>

        <button type="submit">Submit Booking + Pay $50 Deposit</button>
      </form>
    </div>
  </section>

  <section id="info">
    <h2>Rental Info</h2>
    <p><strong>Deposit:</strong> $50 non-refundable required to reserve</p>
    <p><strong>Service Area:</strong> Bristol, MA only</p>
    <p><strong>Availability:</strong> Weekends only. Overnight rental available.</p>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <p>📞 Mark Galan: 774-301-6499</p>
    <p>📞 Kelsey Galan: 774-770-8057</p>
  </section>

  <footer>
    &copy; 2025 M&K Bouncy Houses — All Rights Reserved
  </footer>

  <script>
    document.getElementById('bookingForm').addEventListener('submit', function(e) {
      e.preventDefault();
      alert("This would process the booking & open Stripe payment for deposit.");
    });
  </script>
</body>
</html>
