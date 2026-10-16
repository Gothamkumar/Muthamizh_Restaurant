<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Muthamizh Restaurant | Taste & Enjoy Every Meal</title>

<meta name="description"
content="Welcome to Muthamizh Restaurant. Enjoy delicious biryani, Indian breads, Chinese food, tandoori and more.">

<style>
:root {
    --gold: #eab308;
    --black: #080808;
    --white: #ffffff;
    --cream: #fff9eb;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    background: var(--black);
    color: var(--white);
    line-height: 1.7;
}

header {
    background: #050505;
    padding: 15px 7%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid #b58a13;
    position: sticky;
    top: 0;
    z-index: 1000;
}

.brand {
    display: flex;
    align-items: center;
    gap: 12px;
}

.brand img {
    width: 65px;
    height: 65px;
    object-fit: contain;
}

.brand h2 {
    color: var(--gold);
    font-size: 20px;
}

nav {
    display: flex;
    gap: 22px;
    flex-wrap: wrap;
}

nav a {
    text-decoration: none;
    color: white;
    font-size: 14px;
    transition: .3s;
}

nav a:hover {
    color: var(--gold);
}

.hero {
    min-height: 580px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 60px 20px;
    background:
      linear-gradient(rgba(0,0,0,.72), rgba(0,0,0,.85)),
      url("https://images.unsplash.com/photo-1546833999-b9f581a1996d?auto=format&fit=crop&w=1800&q=85")
      center/cover;
}

.hero-content {
    max-width: 850px;
}

.hero img {
    width: 180px;
    height: 180px;
    object-fit: contain;
    margin-bottom: 10px;
}

.hero h1 {
    font-size: clamp(36px, 6vw, 65px);
    color: var(--gold);
    line-height: 1.2;
}

.hero h3 {
    font-size: 23px;
    margin: 15px 0;
}

.hero p {
    font-size: 17px;
    margin-bottom: 28px;
}

.button {
    display: inline-block;
    background: var(--gold);
    color: #080808;
    padding: 12px 25px;
    border-radius: 5px;
    text-decoration: none;
    font-weight: bold;
    margin: 5px;
    border: 1px solid var(--gold);
    cursor: pointer;
    transition: .3s;
}

.button:hover {
    background: transparent;
    color: var(--gold);
}

.button-outline {
    background: transparent;
    color: var(--gold);
}

section {
    padding: 75px 7%;
    scroll-margin-top: 90px;
}

.section-title {
    text-align: center;
    margin-bottom: 40px;
}

.section-title h2 {
    color: var(--gold);
    font-size: 35px;
}

.section-title p {
    color: #cccccc;
    margin-top: 8px;
}

.about {
    background: #111111;
}

.about-content {
    max-width: 950px;
    margin: auto;
    text-align: center;
}

.about-content p {
    color: #dddddd;
    margin-bottom: 18px;
}

.highlight {
    color: var(--gold);
    font-weight: bold;
}

.info-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
    margin-top: 35px;
}

.info-card {
    border: 1px solid #5d4915;
    border-radius: 10px;
    padding: 25px 15px;
    text-align: center;
    background: #151515;
}

.info-card h3 {
    color: var(--gold);
    margin-bottom: 8px;
}

.menu-section {
    background: #080808;
}

.menu-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
    gap: 22px;
    max-width: 1200px;
    margin: auto;
}

.menu-card {
    background: #141414;
    border: 1px solid #403514;
    border-radius: 10px;
    padding: 25px;
    transition: .3s;
}

.menu-card:hover {
    transform: translateY(-5px);
    border-color: var(--gold);
}

.menu-card h3 {
    color: var(--gold);
    font-size: 22px;
    margin-bottom: 12px;
    border-bottom: 1px solid #514318;
    padding-bottom: 10px;
}

.menu-card ul {
    list-style: none;
}

.menu-card li {
    padding: 5px 0;
    color: #eeeeee;
}

.menu-card li::before {
    content: "✦ ";
    color: var(--gold);
}

.menu-note {
    text-align: center;
    color: #cccccc;
    margin-top: 25px;
}

.events {
    background: #111111;
}

.event-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
    gap: 20px;
    max-width: 1100px;
    margin: auto;
}

.event-card {
    text-align: center;
    padding: 28px 20px;
    background: #191919;
    border-radius: 10px;
    border-bottom: 3px solid var(--gold);
}

.event-card .icon {
    font-size: 38px;
}

.event-card h3 {
    color: var(--gold);
    margin: 10px 0;
}

.booking {
    background: #080808;
}

.booking-form {
    max-width: 700px;
    margin: auto;
    background: #141414;
    padding: 30px;
    border-radius: 12px;
    border: 1px solid #514318;
}

.form-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 18px;
}

.form-group {
    display: flex;
    flex-direction: column;
}

.form-group.full {
    grid-column: 1 / -1;
}

label {
    margin-bottom: 6px;
    color: var(--gold);
}

input, select, textarea {
    width: 100%;
    padding: 12px;
    border-radius: 5px;
    border: 1px solid #555;
    background: #080808;
    color: white;
    font: inherit;
}

textarea {
    resize: vertical;
}

.booking-form button {
    width: 100%;
    margin: 20px 0 0;
    font-size: 16px;
}

.contact {
    background: #111111;
    text-align: center;
}

.contact p {
    margin: 12px 0;
}

.contact a {
    color: var(--gold);
    text-decoration: none;
}

footer {
    background: #030303;
    border-top: 1px solid #574514;
    padding: 30px 15px;
    text-align: center;
    color: #bbbbbb;
}

footer strong {
    color: var(--gold);
}

.whatsapp-float {
    position: fixed;
    right: 20px;
    bottom: 20px;
    background: #25D366;
    color: white;
    padding: 13px 18px;
    border-radius: 50px;
    text-decoration: none;
    font-weight: bold;
    z-index: 2000;
    box-shadow: 0 3px 12px #0008;
}

@media (max-width: 800px) {
    header {
        flex-direction: column;
        gap: 12px;
    }

    nav {
        justify-content: center;
        gap: 13px;
    }

    .brand h2 {
        font-size: 18px;
    }

    section {
        padding: 55px 5%;
    }
}

@media (max-width: 500px) {
    .form-grid {
        grid-template-columns: 1fr;
    }

    .form-group.full {
        grid-column: auto;
    }

    .hero {
        min-height: 500px;
    }

    .hero img {
        width: 140px;
        height: 140px;
    }

    .section-title h2 {
        font-size: 29px;
    }

    .booking-form {
        padding: 20px;
    }
}
</style>
</head>

<body>

<!-- HEADER -->
<header>
    <div class="brand">
        <img src="logo.png" alt="Muthamizh Restaurant Logo">
        <h2>MUTHAMIZH RESTAURANT</h2>
    </div>

    <nav>
        <a href="#home">Home</a>
        <a href="#about">About Us</a>
        <a href="#menu">Menu</a>
        <a href="#events">Events</a>
        <a href="#booking">Pre-Booking</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<!-- HOME -->
<section class="hero" id="home">
    <div class="hero-content">

        <img src="logo.png" alt="Muthamizh Restaurant Logo">

        <h1>Muthamizh Restaurant</h1>

        <h3>Taste the Tradition. Enjoy Every Meal.</h3>

        <p>
            Delicious food, memorable moments, and the joy of dining
            together. Welcome to your family restaurant!
        </p>

        <a class="button" href="#menu">Explore Our Menu</a>

        <a class="button button-outline" href="#booking">
            Book a Table
        </a>

    </div>
</section>

<!-- ABOUT US -->
<section class="about" id="about">

    <div class="section-title">
        <h2>About Us</h2>
        <p>A little story behind every delicious meal.</p>
    </div>

    <div class="about-content">

        <p>
            Welcome to <span class="highlight">Muthamizh Restaurant</span>,
            a place where delicious food brings people together.
        </p>

        <p>
            Started on <span class="highlight">03 July 2026</span>,
            Muthamizh Restaurant was established by a group of friends
            who share a passion for food, hospitality, and creating
            wonderful dining experiences.
        </p>

        <p>
            Our aim is to serve delicious meals in a welcoming atmosphere
            where friends and families can sit together, share happiness,
            and create unforgettable memories.
        </p>

        <p>
            From flavourful biryani and sizzling Chinese dishes to
            traditional Indian breads, tasty gravies, and refreshing
            desserts, we offer a variety of choices for every food lover.
        </p>

        <p class="highlight">
            Our Promise: Good Food. Great Taste. Happy Memories.
        </p>

        <div class="info-grid">

            <div class="info-card">
                <h3>Our Beginning</h3>
                <p>03 July 2026</p>
            </div>

            <div class="info-card">
                <h3>Our Inspiration</h3>
                <p>Friends united by a passion for food.</p>
            </div>

            <div class="info-card">
                <h3>Our Mission</h3>
                <p>Make every meal a memorable experience.</p>
            </div>

        </div>
    </div>
</section>

<!-- MENU -->
<section class="menu-section" id="menu">

    <div class="section-title">
        <h2>Our Menu</h2>
        <p>Discover your favourites at Muthamizh Restaurant.</p>
    </div>

    <div class="menu-grid">

        <div class="menu-card">
            <h3>🍚 Biriyani</h3>
            <ul>
                <li>Plain Biriyani</li>
                <li>Egg Biriyani</li>
                <li>Chicken Biriyani</li>
                <li>Bucket Biriyani</li>
                <li>Medium Bucket — Serves 5–6</li>
                <li>Large Bucket — Serves 7–8</li>
            </ul>
        </div>

        <div class="menu-card">
            <h3>🥡 Chinese Rice & Noodles</h3>
            <ul>
                <li>Veg Rice / Noodles</li>
                <li>Egg Rice / Noodles</li>
                <li>Mushroom Rice / Noodles</li>
                <li>Baby Corn Rice / Noodles</li>
                <li>Paneer Rice / Noodles</li>
                <li>Chicken Rice / Noodles</li>
                <li>Schezwan Rice / Noodles</li>
            </ul>
        </div>

        <div class="menu-card">
            <h3>🍗 Chicken Gravies</h3>
            <ul>
                <li>Butter Chicken</li>
                <li>Pepper Chicken</li>
                <li>Chettinad Chicken</li>
                <li>Pallipalayam Chicken</li>
                <li>Hyderabadi Chicken</li>
                <li>Kadai Chicken Gravy</li>
                <li>Chicken Tikka Masala</li>
                <li>Chicken Do Pyaza</li>
            </ul>
        </div>

        <div class="menu-card">
            <h3>🥦 Veg Gravies</h3>
            <ul>
                <li>Paneer Butter Masala</li>
                <li>Mushroom Masala</li>
                <li>Gobi Masala</li>
                <li>Mixed Vegetable Curry</li>
                <li>Green Peas Masala</li>
            </ul>
        </div>

        <div class="menu-card">
            <h3>🔥 Tandoori & Kebabs</h3>
            <ul>
                <li>Tandoori Chicken</li>
                <li>Tandoori Pepper Chicken</li>
                <li>Chicken Tikka Kebab</li>
                <li>Tangdi Kebab</li>
                <li>Malai Chicken Tikka</li>
                <li>Hariyali Chicken Tikka</li>
                <li>Fish Tikka</li>
                <li>Prawn Tikka</li>
            </ul>
        </div>

        <div class="menu-card">
            <h3>🫓 Indian Breads</h3>
            <ul>
                <li>Plain Naan / Roti / Kulcha</li>
                <li>Butter Naan / Kulcha</li>
                <li>Garlic Naan / Roti</li>
                <li>Tandoori Parotta</li>
                <li>Lachha Paratha</li>
                <li>Pudina Paratha</li>
                <li>Phulka</li>
            </ul>
        </div>

        <div class="menu-card">
            <h3>🥗 Veg Starters</h3>
            <ul>
                <li>Mushroom 65</li>
                <li>Gobi 65</li>
                <li>Paneer 65</li>
                <li>Baby Corn 65</li>
            </ul>
        </div>

        <div class="menu-card">
            <h3>🍗 Non-Veg Starters</h3>
            <ul>
                <li>Chicken 65</li>
                <li>Fish 65 / Prawn 65</li>
                <li>Pepper Fry</li>
                <li>Dragon Chicken</li>
                <li>Chilli Chicken</li>
                <li>Chicken Manchurian</li>
                <li>Hot Pepper Chicken</li>
                <li>Honey Chicken</li>
                <li>Lemon Chicken</li>
                <li>Chicken Lollipop</li>
            </ul>
        </div>

        <div class="menu-card">
            <h3>🍲 Soups</h3>
            <ul>
                <li>Veg Clear Soup</li>
                <li>Veg Hot & Sour Soup</li>
                <li>Veg Manchow Soup</li>
                <li>Non-Veg Clear Soup</li>
                <li>Non-Veg Hot & Sour Soup</li>
                <li>Non-Veg Manchow Soup</li>
            </ul>
        </div>

        <div class="menu-card">
            <h3>🍳 Egg Specials</h3>
            <ul>
                <li>Half Boil</li>
                <li>Boiled Egg</li>
                <li>Omelette</li>
                <li>Egg Kalakki</li>
                <li>Egg Podimas</li>
                <li>Egg Gravy</li>
            </ul>
        </div>

        <div class="menu-card">
            <h3>🍨 Desserts & Drinks</h3>
            <ul>
                <li>Gulab Jamun</li>
                <li>Ice Cream</li>
                <li>Soda</li>
                <li>Coca-Cola</li>
                <li>Water Bottle</li>
            </ul>
        </div>

    </div>

    <p class="menu-note">
        Menu availability and prices may vary. Please contact us for details.
    </p>

    <div style="text-align:center; margin-top:25px;">
        <a class="button" href="#booking">Plan Your Visit</a>
    </div>

</section>

<!-- EVENTS -->
<section class="events" id="events">

    <div class="section-title">
        <h2>Celebrate With Us</h2>
        <p>Good food makes every celebration special.</p>
    </div>

    <div class="event-grid">

        <div class="event-card">
            <div class="icon">🎂</div>
            <h3>Birthday Parties</h3>
            <p>Celebrate special birthdays with family, friends and delicious food.</p>
        </div>

        <div class="event-card">
            <div class="icon">👨‍👩‍👧‍👦</div>
            <h3>Family Gatherings</h3>
            <p>Bring everyone together and enjoy a memorable meal.</p>
        </div>

        <div class="event-card">
            <div class="icon">🎉</div>
            <h3>Special Occasions</h3>
            <p>Contact us to discuss your celebration and food requirements.</p>
        </div>

    </div>

    <div style="text-align:center; margin-top:30px;">
        <a class="button"
           href="https://wa.me/916369689798?text=Hello%20Muthamizh%20Restaurant%2C%20I%20would%20like%20to%20enquire%20about%20an%20event.">
            Enquire About Events
        </a>
    </div>

</section>

<!-- TABLE PRE-BOOKING -->
<section class="booking" id="booking">

    <div class="section-title">
        <h2>Pre-Book Your Table</h2>
        <p>Planning a meal with friends or family? Send us your booking request.</p>
    </div>

    <form class="booking-form" id="bookingForm">

        <div class="form-grid">

            <div class="form-group">
                <label for="customerName">Your Name *</label>
                <input id="customerName" type="text" required
                       placeholder="Enter your name">
            </div>

            <div class="form-group">
                <label for="phone">Mobile Number *</label>
                <input id="phone" type="tel" required
                       pattern="[0-9]{10}"
                       maxlength="10"
                       placeholder="10-digit mobile number">
            </div>

            <div class="form-group">
                <label for="date">Booking Date *</label>
                <input id="date" type="date" required>
            </div>

            <div class="form-group">
                <label for="time">Preferred Time *</label>
                <input id="time" type="time" required>
            </div>

            <div class="form-group">
                <label for="guests">Number of Guests *</label>
                <select id="guests" required>
                    <option value="">Select guests</option>
                    <option>1</option>
                    <option>2</option>
                    <option>3</option>
                    <option>4</option>
                    <option>5</option>
                    <option>6</option>
                    <option>7</option>
                    <option>8</option>
                    <option>More than 8</option>
                </select>
            </div>

            <div class="form-group">
                <label for="occasion">Occasion</label>
                <select id="occasion">
                    <option>Regular Dining</option>
                    <option>Birthday</option>
                    <option>Family Gathering</option>
                    <option>Special Occasion</option>
                    <option>Other</option>
                </select>
            </div>

            <div class="form-group full">
                <label for="requests">Special Requests</label>
                <textarea id="requests" rows="3"
                          placeholder="Any special requirements?"></textarea>
            </div>

        </div>

        <button class="button" type="submit">
            Send Booking Request on WhatsApp
        </button>

        <p style="color:#ccc; font-size:13px; margin-top:12px;">
            Your booking is a request, not a confirmed reservation.
            We will confirm availability through WhatsApp.
        </p>

    </form>

</section>

<!-- CONTACT -->
<section class="contact" id="contact">

    <div class="section-title">
        <h2>Visit Muthamizh Restaurant</h2>
        <p>We look forward to serving you!</p>
    </div>

    <p>📞 Phone: <a href="tel:+916369689798">63696 89798</a></p>

    <p>📱 Instagram:
       <a href="https://www.instagram.com/muthamizh_restaurant/"
          target="_blank" rel="noopener">
          @muthamizh_restaurant
       </a>
    </p>

    <p>📍 Location: Punjaipuliampatti, Tamil Nadu</p>

    <p>📅 Established: 03 July 2026</p>

    <div style="margin-top:25px;">
        <a class="button"
           href="https://wa.me/916369689798"
           target="_blank" rel="noopener">
           Contact Us on WhatsApp
        </a>
    </div>

</section>

<!-- FOOTER -->
<footer>
    <p><strong>MUTHAMIZH RESTAURANT</strong></p>

    <p>Taste the Tradition. Enjoy Every Meal.</p>

    <p>Your Opinion = Our Motivation ❤️</p>

    <p style="margin-top:15px;">
        &copy; <span id="year"></span> Muthamizh Restaurant.
        All Rights Reserved.
    </p>
</footer>

<!-- WHATSAPP FLOAT BUTTON -->
<a class="whatsapp-float"
   href="https://wa.me/916369689798"
   target="_blank" rel="noopener"
   aria-label="Contact Muthamizh Restaurant on WhatsApp">
   WhatsApp
</a>

<script>
document.getElementById("year").textContent =
    new Date().getFullYear();

// Prevent selecting past booking dates.
const dateInput = document.getElementById("date");
const today = new Date();
const localToday = [
    today.getFullYear(),
    String(today.getMonth() + 1).padStart(2, "0"),
    String(today.getDate()).padStart(2, "0")
].join("-");

dateInput.min = localToday;

// Send table booking details to WhatsApp.
document.getElementById("bookingForm").addEventListener("submit", function(e) {
    e.preventDefault();

    const name = document.getElementById("customerName").value.trim();
    const phone = document.getElementById("phone").value.trim();
    const date = document.getElementById("date").value;
    const time = document.getElementById("time").value;
    const guests = document.getElementById("guests").value;
    const occasion = document.getElementById("occasion").value;
    const requests = document.getElementById("requests").value.trim();

    if (!/^[0-9]{10}$/.test(phone)) {
        alert("Please enter a valid 10-digit mobile number.");
        return;
    }

    const message =
`Hello Muthamizh Restaurant!

I would like to request a table booking.

Name: ${name}
Mobile: ${phone}
Date: ${date}
Preferred Time: ${time}
Number of Guests: ${guests}
Occasion: ${occasion}
Special Requests: ${requests || "None"}

Please confirm table availability. Thank you!`;

    const whatsappURL =
        "https://wa.me/916369689798?text=" + encodeURIComponent(message);

    window.open(whatsappURL, "_blank");
});
</script>

</body>
</html>
