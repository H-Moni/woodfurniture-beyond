# woodfurniture-beyond
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Wood, Furniture & Beyond - Premium wooden furniture and interior solutions in Islampur, Jamalpur, Bangladesh. Custom beds, sofas, dining tables, and more since 1997.">
    <meta name="keywords" content="furniture, wooden furniture, bed, sofa, dining table, Islampur, Jamalpur, Bangladesh, custom furniture">
    <title>Wood, Furniture & Beyond | Premium Wooden Furniture in Islampur, Jamalpur</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, #8B4513 0%, #D2691E 100%);
            color: white;
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        nav {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            transition: opacity 0.3s;
        }

        nav a:hover {
            opacity: 0.8;
        }

        .mobile-menu {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #8B4513 0%, #D2691E 100%);
            color: white;
            padding: 4rem 2rem;
            text-align: center;
        }

        .hero-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
        }

        .cta-button {
            display: inline-block;
            background: white;
            color: #8B4513;
            padding: 1rem 2rem;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            transition: transform 0.3s;
        }

        .cta-button:hover {
            transform: scale(1.05);
        }

        /* Sections */
        section {
            max-width: 1200px;
            margin: 0 auto;
            padding: 4rem 2rem;
        }

        h2 {
            font-size: 2.5rem;
            margin-bottom: 2rem;
            text-align: center;
            color: #8B4513;
        }

        /* About */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .about-text {
            font-size: 1.1rem;
        }

        .about-info {
            background: #f9f9f9;
            padding: 2rem;
            border-radius: 10px;
            border-left: 4px solid #8B4513;
        }

        .about-info h3 {
            color: #8B4513;
            margin-bottom: 1rem;
        }

        .about-info p {
            margin-bottom: 0.5rem;
        }

        /* Products */
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .product-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .product-card:hover {
            transform: translateY(-5px);
        }

        .product-icon {
            background: linear-gradient(135deg, #8B4513 0%, #D2691E 100%);
            color: white;
            padding: 3rem;
            text-align: center;
            font-size: 3rem;
        }

        .product-info {
            padding: 1.5rem;
        }

        .product-info h3 {
            color: #8B4513;
            margin-bottom: 0.5rem;
        }

        /* Calculator */
        .calculator-container {
            background: #f9f9f9;
            padding: 2rem;
            border-radius: 10px;
            max-width: 600px;
            margin: 2rem auto;
        }

        .calc-group {
            margin-bottom: 1.5rem;
        }

        .calc-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: bold;
            color: #8B4513;
        }

        .calc-group select,
        .calc-group input {
            width: 100%;
            padding: 0.75rem;
            border: 2px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }

        .calc-result {
            background: white;
            padding: 1.5rem;
            border-radius: 5px;
            margin-top: 1rem;
            text-align: center;
            border: 2px solid #8B4513;
        }

        .calc-result h3 {
            color: #8B4513;
            font-size: 1.5rem;
        }

        .calc-result p {
            font-size: 2rem;
            color: #D2691E;
            font-weight: bold;
            margin-top: 0.5rem;
        }

        /* Contact */
        .contact-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            margin-top: 2rem;
        }

        .contact-info {
            background: #f9f9f9;
            padding: 2rem;
            border-radius: 10px;
        }

        .contact-item {
            display: flex;
            align-items: start;
            margin-bottom: 1.5rem;
        }

        .contact-item-icon {
            font-size: 1.5rem;
            margin-right: 1rem;
            color: #8B4513;
        }

        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 0.75rem;
            margin-bottom: 1rem;
            border: 2px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }

        .contact-form button {
            background: #8B4513;
            color: white;
            padding: 1rem 2rem;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            cursor: pointer;
            transition: background 0.3s;
        }

        .contact-form button:hover {
            background: #D2691E;
        }

        /* Footer */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 2rem;
        }

        .social-links {
            margin-top: 1rem;
        }

        .social-links a {
            color: white;
            margin: 0 1rem;
            font-size: 1.5rem;
            text-decoration: none;
        }

        /* Responsive */
        @media (max-width: 768px) {
            nav ul {
                display: none;
            }

            .mobile-menu {
                display: block;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .about-content,
            .contact-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <nav>
            <div class="logo">Wood, Furniture & Beyond</div>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#calculator">Price Calculator</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="mobile-menu">☰</div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Wood, Furniture & Beyond</h1>
            <p>We Shape Your Dreamy Wooden Interior With Responsibility and Care</p>
            <p style="font-size: 1rem; margin-bottom: 1rem;">SINCE 1997 | ESTD 1997</p>
            <a href="#contact" class="cta-button">Get a Quote Today</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2>About Us</h2>
        <div class="about-content">
            <div class="about-text">
                <p style="margin-bottom: 1rem;">Welcome to Wood, Furniture & Beyond, your trusted partner in creating beautiful wooden interiors since 1997. With over 25 years of experience, we have been serving the community of Islampur, Jamalpur, and surrounding areas with premium quality furniture and wooden products.</p>
                <p style="margin-bottom: 1rem;">We specialize in custom-made furniture that perfectly fits your space and style. Our skilled craftsmen use only the finest quality wood to create durable, elegant pieces that stand the test of time.</p>
                <p>From concept to completion, we work closely with our clients to bring their vision to life, ensuring every piece reflects their unique taste and requirements.</p>
            </div>
            <div class="about-info">
                <h3>Business Information</h3>
                <p><strong>Owner:</strong> Md. Hafijur Rahman</p>
                <p><strong>Established:</strong> 1997</p>
                <p><strong>Location:</strong> West to Islampur Fire Service Office, Islampur, Jamalpur, Bangladesh</p>
                <p><strong>Experience:</strong> 25+ Years</p>
                <p><strong>Specialty:</strong> Custom Wooden Furniture & Interior Design</p>
            </div>
        </div>
    </section>

    <!-- Products Section -->
    <section id="products">
        <h2>Our Products</h2>
        <div class="products-grid">
            <div class="product-card">
                <div class="product-icon">🪵</div>
                <div class="product-info">
                    <h3>Fine & Raw Wood</h3>
                    <p>Premium quality fine wood and raw wood materials for all your carpentry needs.</p>
                </div>
            </div>
            <div class="product-card">
                <div class="product-icon">🛏️</div>
                <div class="product-info">
                    <h3>Beds</h3>
                    <p>Comfortable and stylish beds in various sizes and designs to suit your bedroom.</p>
                </div>
            </div>
            <div class="product-card">
                <div class="product-icon">🛋️</div>
                <div class="product-info">
                    <h3>Sofas</h3>
                    <p>Elegant sofas and seating solutions for your living room comfort.</p>
                </div>
            </div>
            <div class="product-card">
                <div class="product-icon">🍽️</div>
                <div class="product-info">
                    <h3>Dining Tables</h3>
                    <p>Beautiful dining tables that bring families together for memorable meals.</p>
                </div>
            </div>
            <div class="product-card">
                <div class="product-icon">📚</div>
                <div class="product-info">
                    <h3>Study Tables</h3>
                    <p>Functional study tables perfect for students and professionals.</p>
                </div>
            </div>
            <div class="product-card">
                <div class="product-icon">🪑</div>
                <div class="product-info">
                    <h3>Chairs</h3>
                    <p>Comfortable chairs for dining, office, or decorative purposes.</p>
                </div>
            </div>
            <div class="product-card">
                <div class="product-icon">🗄️</div>
                <div class="product-info">
                    <h3>Cabinets & Racks</h3>
                    <p>Storage solutions including cabinets and racks for organized living.</p>
                </div>
            </div>
            <div class="product-card">
                <div class="product-icon">💄</div>
                <div class="product-info">
                    <h3>Dressing Tables</h3>
                    <p>Elegant dressing tables with mirrors for your grooming needs.</p>
                </div>
            </div>
            <div class="product-card">
                <div class="product-icon">👔</div>
                <div class="product-info">
                    <h3>Wardrobes</h3>
                    <p>Spacious wardrobes to keep your clothes organized and protected.</p>
                </div>
            </div>
            <div class="product-card">
                <div class="product-icon">🏠</div>
                <div class="product-info">
                    <h3>Wooden Interiors</h3>
                    <p>Complete wooden interior solutions for homes and offices.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Price Calculator Section -->
    <section id="calculator">
        <h2>Price Calculator</h2>
        <p style="text-align: center; margin-bottom: 2rem;">Get an estimated price for your furniture. Final prices may vary based on wood quality, design complexity, and customization.</p>
        <div class="calculator-container">
            <div class="calc-group">
                <label for="product-type">Select Product Type:</label>
                <select id="product-type">
                    <option value="">-- Choose Product --</option>
                    <option value="bed">Bed</option>
                    <option value="sofa">Sofa</option>
                    <option value="dining">Dining Table</option>
                    <option value="study">Study Table</option>
                    <option value="chair">Chair</option>
                    <option value="cabinet">Cabinet</option>
                    <option value="rack">Rack</option>
                    <option value="dressing">Dressing Table</option>
                    <option value="wardrobe">Wardrobe</option>
                </select>
            </div>
            <div class="calc-group">
                <label for="wood-type">Wood Quality:</label>
                <select id="wood-type">
                    <option value="">-- Choose Wood Type --</option>
                    <option value="economy">Economy (Softwood)</option>
                    <option value="standard">Standard (Seasoned Wood)</option>
                    <option value="premium">Premium (Hardwood)</option>
                    <option value="luxury">Luxury (Teak/Mahogany)</option>
                </select>
            </div>
            <div class="calc-group">
                <label for="size">Size (in feet):</label>
                <input type="number" id="size" placeholder="Enter approximate size" min="1">
            </div>
            <div class="calc-group">
                <label for="quantity">Quantity:</label>
                <input type="number" id="quantity" placeholder="Number of items" min="1" value="1">
            </div>
            <div class="calc-result" id="result" style="display: none;">
                <h3>Estimated Price</h3>
                <p id="price-output">৳ 0</p>
                <small style="color: #666;">*This is an approximate estimate. Contact us for accurate pricing.</small>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Us</h2>
        <div class="contact-grid">
            <div class="contact-info">
                <h3 style="color: #8B4513; margin-bottom: 1.5rem;">Get In Touch</h3>
                <div class="contact-item">
                    <div class="contact-item-icon">👤</div>
                    <div>
                        <strong>Owner</strong><br>
                        Md. Hafijur Rahman
                    </div>
                </div>
                <div class="contact-item">
                    <div class="contact-item-icon">📍</div>
                    <div>
                        <strong>Location</strong><br>
                        West to Islampur Fire Service Office<br>
                        Islampur, Jamalpur, Bangladesh
                    </div>
                </div>
                <div class="contact-item">
                    <div class="contact-item-icon">📱</div>
                    <div>
                        <strong>Phone</strong><br>
                        +880 1XXX-XXXXXX
                    </div>
                </div>
                <div class="contact-item">
                    <div class="contact-item-icon">✉️</div>
                    <div>
                        <strong>Email</strong><br>
                        info@woodfurniturebeyond.com
                    </div>
                </div>
                <div class="contact-item">
                    <div class="contact-item-icon">🕒</div>
                    <div>
                        <strong>Business Hours</strong><br>
                        Saturday - Thursday: 9:00 AM - 8:00 PM<br>
                        Friday: Closed
                    </div>
                </div>
            </div>
            <div class="contact-form">
                <h3 style="color: #8B4513; margin-bottom: 1.5rem;">Send us a Message</h3>
                <form id="contactForm">
                    <input type="text" placeholder="Your Name" required>
                    <input type="tel" placeholder="Your Phone" required>
                    <input type="email" placeholder="Your Email">
                    <textarea rows="5" placeholder="Your Message" required></textarea>
                    <button type="submit">Send Message</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Wood, Furniture & Beyond. All Rights Reserved.</p>
        <p>Established 1997 | 25+ Years of Excellence</p>
        <div class="social-links">
            <a href="https://facebook.com" target="_blank">📘 Facebook</a>
            <a href="https://wa.me/880XXXXXXXXXX" target="_blank">💬 WhatsApp</a>
        </div>
        <p style="margin-top: 1rem; font-size: 0.9rem;">West to Islampur Fire Service Office, Islampur, Jamalpur, Bangladesh</p>
    </footer>

    <script>
        // Price Calculator Logic
        const priceData = {
            bed: { base: 15000, multiplier: 2000 },
            sofa: { base: 12000, multiplier: 1800 },
            dining: { base: 20000, multiplier: 2500 },
            study: { base: 8000, multiplier: 1200 },
            chair: { base: 2500, multiplier: 500 },
            cabinet: { base: 10000, multiplier: 1500 },
            rack: { base: 6000, multiplier: 800 },
            dressing: { base: 12000, multiplier: 1800 },
            wardrobe: { base: 25000, multiplier: 3000 }
        };

        const woodMultiplier = {
            economy: 1,
            standard: 1.3,
            premium: 1.7,
            luxury: 2.5
        };

        function calculatePrice() {
            const product = document.getElementById('product-type').value;
            const wood = document.getElementById('wood-type').value;
            const size = parseFloat(document.getElementById('size').value) || 0;
            const quantity = parseInt(document.getElementById('quantity').value) || 1;

            if (product && wood && size > 0) {
                const basePrice = priceData[product].base;
                const sizePrice = priceData[product].multiplier * size;
                const woodPrice = (basePrice + sizePrice) * woodMultiplier[wood];
                const totalPrice = woodPrice * quantity;

                document.getElementById('price-output').textContent = 
                    '৳ ' + totalPrice.toLocaleString('en-BD', { maximumFractionDigits: 0 });
                document.getElementById('result').style.display = 'block';
            }
        }

        document.getElementById('product-type').addEventListener('change', calculatePrice);
        document.getElementById('wood-type').addEventListener('change', calculatePrice);
        document.getElementById('size').addEventListener('input', calculatePrice);
        document.getElementById('quantity').addEventListener('input', calculatePrice);

        // Form Submission
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! We will contact you soon.');
            this.reset();
        });

        // Smooth Scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });
    </script>
</body>
</html>
