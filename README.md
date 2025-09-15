# Ray-Romano-contracting-website-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Ray Romano Contracting - Home Renovations NYC & Hamptons</title>
    <style>
        /* Reset and base */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            background: #f9f9f9;
            color: #333;
            line-height: 1.6;
        }
        a {
            color: #0077cc;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
        header {
            background: #004d40;
            color: white;
            padding: 20px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        header h1 {
            font-size: 1.8rem;
            letter-spacing: 2px;
        }
        nav a {
            margin-left: 25px;
            font-weight: 600;
            font-size: 1rem;
        }
        .hero {
            background: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1350&q=80') no-repeat center center/cover;
            height: 600px;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
            padding: 0 20px;
        }
        .hero h2 {
            font-size: 3rem;
            text-shadow: 2px 2px 8px rgba(0,0,0,0.7);
            max-width: 900px;
        }
        .container {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
        }
        h2.section-title {
            text-align: center;
            margin-bottom: 30px;
            font-size: 2.5rem;
            color: #004d40;
            letter-spacing: 1.5px;
        }
        .services, .models, .testimonials {
            display: grid;
            grid-template-columns: repeat(auto-fit,minmax(280px,1fr));
            gap: 30px;
        }
        .service-card, .model-card, .testimonial-card {
            background: white;
            border-radius: 10px;
            box-shadow: 0 6px 15px rgba(0,0,0,0.1);
            padding: 20px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        .service-card img, .model-card img {
            width: 100%;
            border-radius: 10px;
            height: 180px;
            object-fit: cover;
            margin-bottom: 15px;
        }
        .service-card h3, .model-card h3 {
            color: #00796b;
            margin-bottom: 10px;
        }
        .service-card p, .model-card p {
            flex-grow: 1;
            font-size: 1rem;
            margin-bottom: 15px;
        }
        .price {
            font-weight: 700;
            font-size: 1.2rem;
            color: #d32f2f;
            margin-bottom: 15px;
        }
        button.add-to-cart {
            background: #00796b;
            color: white;
            border: none;
            padding: 12px;
            border-radius: 6px;
            cursor: pointer;
            font-weight: 600;
            transition: background 0.3s ease;
        }
        button.add-to-cart:hover {
            background: #004d40;
        }
        .cart {
            position: fixed;
            right: 20px;
            top: 80px;
            width: 320px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 6px 20px rgba(0,0,0,0.15);
            padding: 20px;
            max-height: 80vh;
            overflow-y: auto;
            z-index: 1100;
        }
        .cart h3 {
            margin-bottom: 15px;
            color: #004d40;
        }
        .cart-item {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
            font-size: 1rem;
        }
        .cart-total {
            font-weight: 700;
            font-size: 1.2rem;
            margin-top: 15px;
            border-top: 1px solid #ddd;
            padding-top: 10px;
            color: #d32f2f;
        }
        .checkout {
            margin-top: 20px;
        }
        .checkout label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
        }
        .checkout select, .checkout input[type="text"], .checkout input[type="email"] {
            width: 100%;
            padding: 8px;
            margin-bottom: 15px;
            border-radius: 6px;
            border: 1px solid #ccc;
            font-size: 1rem;
        }
        .checkout button {
            width: 100%;
            background: #d32f2f;
            color: white;
            border: none;
            padding: 12px;
            border-radius: 6px;
            font-weight: 700;
            cursor: pointer;
            font-size: 1.1rem;
            transition: background 0.3s ease;
        }
        .checkout button:hover {
            background: #9a0007;
        }
        footer {
            background: #004d40;
            color: white;
            text-align: center;
            padding: 20px 10px;
            margin-top: 60px;
            font-size: 0.9rem;
        }
        /* Responsive */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                align-items: flex-start;
            }
            nav {
                margin-top: 10px;
            }
            .cart {
                position: static;
                width: 100%;
                max-height: none;
                margin: 20px 0;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Ray Romano Contracting</h1>
        <nav>
            <a href="#services">Services</a>
            <a href="#models">Models</a>
            <a href="#testimonials">Testimonials</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section class="hero">
        <h2>Renovating Your Dream Home in NYC & The Hamptons for Over 25 Years</h2>
    </section>

    <main class="container">
        <section id="services">
            <h2 class="section-title">Our Services</h2>
            <div class="services">
                <div class="service-card">
                    <img src="https://images.unsplash.com/photo-1560448070-8a1f0a7a7a3a?auto=format&fit=crop&w=600&q=80" alt="Gut Renovation" />
                    <h3>Complete Gut Renovation</h3>
                    <p>Transform your space from the ground up with our expert gut renovation services, tailored to your style and needs.</p>
                    <p class="price">$75,000 - $150,000</p>
                    <button class="add-to-cart" data-name="Complete Gut Renovation" data-price="75000">Add to Cart</button>
                </div>
                <div class="service-card">
                    <img src="https://images.unsplash.com/photo-1505691938895-1758d7feb511?auto=format&fit=crop&w=600&q=80" alt="Kitchen Remodel" />
                    <h3>Kitchen Remodel</h3>
                    <p>Upgrade your kitchen with modern layouts, finishes, and appliances to create a functional and beautiful space.</p>
                    <p class="price">$30,000 - $70,000</p>
                    <button class="add-to-cart" data-name="Kitchen Remodel" data-price="30000">Add to Cart</button>
                </div>
                <div class="service-card">
                    <img src="https://images.unsplash.com/photo-1501183638714-3c3b0e5b0f4a?auto=format&fit=crop&w=600&q=80" alt="Bathroom Renovation" />
                    <h3>Bathroom Renovation</h3>
                    <p>Elegant and efficient bathroom renovations with premium fixtures and custom designs.</p>
                    <p class="price">$20,000 - $50,000</p>
                    <button class="add-to-cart" data-name="Bathroom Renovation" data-price="20000">Add to Cart</button>
                </div>
            </div>
        </section>

        <section id="models" style="margin-top: 60px;">
            <h2 class="section-title">Featured Models & Projects</h2>
            <div class="models">
                <div class="model-card">
                    <img src="https://images.unsplash.com/photo-1494526585095-c41746248156?auto=format&fit=crop&w=600&q=80" alt="Upper West Side Classic 6" />
                    <h3>Upper West Side Classic 6</h3>
                    <p>Complete gut renovation of an eight-room prewar apartment, finished in under 8 weeks.</p>
                    <p class="price">$120,000</p>
                    <button class="add-to-cart" data-name="Upper West Side Classic 6" data-price="120000">Add to Cart</button>
                </div>
                <div class="model-card">
                    <img src="https://images.unsplash.com/photo-1501183638714-3c3b0e5b0f4a?auto=format&fit=crop&w=600&q=80" alt="Hamptons Vacation Home" />
                    <h3>Hamptons Vacation Home</h3>
                    <p>Luxury renovation combining multiple units into a spacious vacation retreat.</p>
                    <p class="price">$200,000</p>
                    <button class="add-to-cart" data-name="Hamptons Vacation Home" data-price="200000">Add to Cart</button>
                </div>
                <div class="model-card">
                    <img src="https://images.unsplash.com/photo-1560448070-8a1f0a7a7a3a?auto=format&fit=crop&w=600&q=80" alt="Madison Avenue Art Gallery" />
                    <h3>Madison Avenue Art Gallery</h3>
                    <p>Custom renovation for a high-end art gallery space with specialized lighting and finishes.</p>
                    <p class="price">$90,000</p>
                    <button class="add-to-cart" data-name="Madison Avenue Art Gallery" data-price="90000">Add to Cart</button>
                </div>
            </div>
        </section>

        <section id="testimonials" style="margin-top: 60px;">
            <h2 class="section-title">What Our Clients Say</h2>
            <div class="testimonials">
                <div class="testimonial-card">
                    <p>"Ray Romano rocks. He did a complete GUT on an eight-room wreck in less than 8 weeks. The place is beautiful!"</p>
                    <strong>- Jamie Floyd, Upper West Side Classic 6</strong>
                </div>
                <div class="testimonial-card">
                    <p>"Ray rescued us from a contractor job gone bad. He and his crew are great, neat and real artisans. Highly recommended!"</p>
                    <strong>- Donna and Scott, Rescued Renovation</strong>
                </div>
                <div class="testimonial-card">
                    <p>"Ray added value in ways that other G.C.s can't. He more than doubled the value of my apartment through his gut renovations."</p>
                    <strong>- David Siegel, Doubled the Value</strong>
                </div>
            </div>
        </section>

        <section id="contact" style="margin-top: 60px;">
            <h2 class="section-title">Contact Us</h2>
            <p style="text-align:center; max-width: 600px; margin: 0 auto 30px auto;">
                For inquiries, consultations, or to schedule a project walkthrough, please email us at 
                <a href="mailto:info@rayromanocontracting.com">info@rayromanocontracting.com</a> or call (212) 555-1234.
            </p>
        </section>
    </main>

    <aside class="cart" id="cart">
        <h3>Your Cart</h3>
        <div id="cart-items">
            <p>Your cart is empty.</p>
        </div>
        <div class="cart-total" id="cart-total"></div>
        <form class="checkout" id="checkout-form" style="display:none;">
            <label for="payment-method">Payment Method</label>
            <select id="payment-method" required>
                <option value="" disabled selected>Select payment method</option>
                <option value="online">Online Payment</option>
                <option value="cod">Cash on Delivery</option>
                <option value="check">Check Payment</option>
            </select>
            <label for="customer-name">Name</label>
            <input type="text" id="customer-name" placeholder="Your full name" required />
            <label for="customer-email">Email</label>
            <input type="email" id="customer-email" placeholder="Your email address" required />
            <button type="submit">Place Order</button>
        </form>
        <p id="order-message" style="color:green; font-weight:bold; display:none; margin-top: 15px;"></p>
    </aside>

    <footer>
        &copy; 2025 Ray Romano Contracting. All rights reserved. | NYC & Hamptons Renovations
    </footer>

    <script>
        <!-- Duplicate script block removed. Use only one script block at the end of the file. -->
    </script>
</body>
</html>
