<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Harbor View Ormoc - Signature Side Dishes</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            background-color: #f8f5f0;
            color: #2d2d2d;
        }
        /* Mobile-First Header */
        .header {
            background-color: #1a3d6f;
            color: white;
            padding: 1.5rem 1rem;
            text-align: center;
        }
        .header small {
            display: block;
            margin-top: 0.5rem;
            font-size: 0.8rem;
            opacity: 0.8;
        }
        /* Mobile Navigation */
        .nav {
            background-color: #2d5b99;
            padding: 1rem;
            overflow-x: auto;
        }
        .nav-list {
            display: flex;
            gap: 1.2rem;
            list-style: none;
        }
        .nav-link {
            color: white;
            text-decoration: none;
            font-weight: 500;
            white-space: nowrap;
        }
        .nav-link.active {
            border-bottom: 2px solid #ffd166;
        }
        /* Side Dish Cards */
        .menu-section {
            padding: 1.5rem 1rem;
        }
        .section-title {
            color: #1a3d6f;
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        .chef-badge {
            background-color: #ffd166;
            color: #1a3d6f;
            font-size: 0.7rem;
            padding: 0.2rem 0.5rem;
            border-radius: 5px;
            font-weight: bold;
        }
        .dishes-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1.2rem;
        }
        .dish-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .dish-img {
            width: 100%;
            height: 150px;
            object-fit: cover;
            background-color: #e0e0e0; /* Placeholder */
        }
        .dish-details {
            padding: 1rem;
        }
        .dish-name {
            color: #1a3d6f;
            margin-bottom: 0.5rem;
        }
        .dish-desc {
            font-size: 0.9rem;
            color: #555;
            margin-bottom: 0.8rem;
            line-height: 1.4;
        }
        .dish-price {
            font-weight: bold;
            color: #2d5b99;
            margin-bottom: 0.8rem;
        }
        .add-btn {
            width: 100%;
            padding: 0.8rem;
            background-color: #ffd166;
            border: none;
            border-radius: 5px;
            font-weight: bold;
            color: #1a3d6f;
            cursor: pointer;
        }
        /* Footer (Hotel Info) */
        .footer {
            background-color: #1a3d6f;
            color: white;
            padding: 1.5rem 1rem;
            text-align: center;
            font-size: 0.9rem;
        }
        .footer p {
            margin-bottom: 0.5rem;
        }
        /* Desktop Breakpoint */
        @media (min-width: 768px) {
            .dishes-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            .nav {
                text-align: center;
            }
            .nav-list {
                justify-content: center;
            }
        }
    </style>
</head>
<body>
    <!-- Hotel Header -->
    <header class="header">
        <h1>Harbor View Ormoc</h1>
        <small>Signature Side Dishes (Pair with Our Coastal Main Courses)</small>
    </header>

    <!-- Category Navigation -->
    <nav class="nav">
        <ul class="nav-list">
            <li><a href="#meat" class="nav-link active">Meat-Infused</a></li>
            <li><a href="#veggie">Vegetarian</a></li>
            <li><a href="#seafood">Seafood-Infused</a></li>
            <li><a href="#chef">Chef's Picks</a></li>
        </ul>
    </nav>

    <!-- Main Menu Sections -->
    <main>
        <!-- Meat-Infused Sides -->
        <section class="menu-section" id="meat">
            <h2 class="section-title">Meat-Infused Sides</h2>
            <div class="dishes-grid">
                <div class="dish-card">
                    <img src="https://via.placeholder.com/300x150?text=Loaded+Mashed+Potatoes" alt="Bacon-Cheddar Loaded Mashed Potatoes" class="dish-img">
                    <div class="dish-details">
                        <h3 class="dish-name">Bacon-Cheddar Loaded Mashed Potatoes</h3>
                        <p class="dish-desc">Creamy Yukon gold potatoes topped with crispy local bacon, sharp cheddar, and chives.</p>
                        <p class="dish-price">₱195</p>
                        <button class="add-btn">Add to Order</button>
                    </div>
                </div>
                <div class="dish-card">
                    <img src="https://via.placeholder.com/300x150?text=Sausage+Stuffed+Cornbread" alt="Sausage-Stuffed Cornbread Muffins" class="dish-img">
                    <div class="dish-details">
                        <h3 class="dish-name">Sausage-Stuffed Cornbread Muffins</h3>
                        <p class="dish-desc">Sweet cornmeal muffins stuffed with spiced local pork sausage and drizzled with honey butter.</p>
                        <p class="dish-price">₱175</p>
                        <button class="add-btn">Add to Order</button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Vegetarian Sides -->
        <section class="menu-section" id="veggie">
            <h2 class="section-title">Vegetarian Sides</h2>
            <div class="dishes-grid">
                <div class="dish-card">
                    <img src="https://via.placeholder.com/300x150?text=Roasted+Asparagus" alt="Lemon-Parm Roasted Asparagus" class="dish-img">
                    <div class="dish-details">
                        <h3 class="dish-name">Lemon-Parm Roasted Asparagus</h3>
                        <p class="dish-desc">Fresh asparagus roasted with olive oil, lemon zest, and grated parmesan.</p>
                        <p class="dish-price">₱145</p>
                        <button class="add-btn">Add to Order</button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Seafood-Infused Sides -->
        <section class="menu-section" id="seafood">
            <h2 class="section-title">Seafood-Infused Sides</h2>
            <div class="dishes-grid">
                <div class="dish-card">
                    <img src="https://via.placeholder.com/300x150?text=Coconut+Lime+Coleslaw" alt="Coconut-Lime Shrimp Coleslaw" class="dish-img">
                    <div class="dish-details">
                        <h3 class="dish-name">Coconut-Lime Shrimp Coleslaw</h3>
                        <p class="dish-desc">Crunchy cabbage mix with grilled local shrimp, coconut milk dressing, and lime juice.</p>
                        <p class="dish-price">₱215</p>
                        <button class="add-btn">Add to Order</button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Chef's Picks -->
        <section class="menu-section" id="chef">
            <h2 class="section-title">Chef's Picks <span class="chef-badge">Limited Daily</span></h2>
            <div class="dishes-grid">
                <div class="dish-card">
                    <img src="https://via.placeholder.com/300x150?text=Truffle+Mac+Cheese" alt="Truffle Mac & Cheese Bites" class="dish-img">
                    <div class="dish-details">
                        <h3 class="dish-name">Truffle Mac & Cheese Bites</h3>
                        <p class="dish-desc">Creamy gouda macaroni coated in panko, fried, and drizzled with black truffle oil.</p>
                        <p class="dish-price">₱235</p>
                        <button class="add-btn">Add to Order</button>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Hotel Footer -->
    <footer class="footer">
        <p>Harbor View Ormoc | Ormoc City, Leyte</p>
        <p>Dining Hours: 6AM - 10PM Daily</p>
        <p>Special Dietary Requests? Ask Our Server!</p>
    </footer>
</body>
</html>
