# Ex02 Commercial Website
## Date:24-11-2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LUXORA — Premium Lifestyle Store</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
</head>
<body>
    <!-- ===================== ANNOUNCEMENT BAR ===================== -->
    <div class="announcement-bar">
        <p><i class="fas fa-truck"></i> Free Shipping on Orders Over $99 &mdash; <a href="#shop">Shop Now</a></p>
    </div>

    <!-- ===================== NAVIGATION ===================== -->
    <header class="header" id="header">
        <nav class="navbar">
            <a href="#" class="logo">
                <span class="logo-icon">◆</span> LUXORA
            </a>

            <ul class="nav-links" id="navLinks">
                <li><a href="#home" class="nav-link active">Home</a></li>
                <li><a href="#shop" class="nav-link">Shop</a></li>
                <li><a href="#collections" class="nav-link">Collections</a></li>
                <li><a href="#about" class="nav-link">About</a></li>
                <li><a href="#testimonials" class="nav-link">Reviews</a></li>
                <li><a href="#contact" class="nav-link">Contact</a></li>
            </ul>

            <div class="nav-actions">
                <button class="nav-icon-btn" aria-label="Search" id="searchBtn">
                    <i class="fas fa-search"></i>
                </button>
                <button class="nav-icon-btn" aria-label="Wishlist">
                    <i class="fas fa-heart"></i>
                    <span class="badge">3</span>
                </button>
                <button class="nav-icon-btn" aria-label="Cart" id="cartBtn">
                    <i class="fas fa-shopping-bag"></i>
                    <span class="badge" id="cartCount">2</span>
                </button>
                <button class="hamburger" id="hamburger" aria-label="Menu">
                    <span></span><span></span><span></span>
                </button>
            </div>
        </nav>

        <!-- Search Overlay -->
        <div class="search-overlay" id="searchOverlay">
            <div class="search-container">
                <input type="text" placeholder="Search products, collections..." class="search-input" id="searchInput">
                <button class="search-close" id="searchClose"><i class="fas fa-times"></i></button>
            </div>
        </div>
    </header>

    <!-- ===================== HERO SECTION ===================== -->
    <section class="hero" id="home">
        <div class="hero-bg">
            <img src="https://images.unsplash.com/photo-1441986300917-64674bd600d8?w=1920&q=80" alt="Luxury Store" class="hero-bg-img">
            <div class="hero-overlay"></div>
        </div>
        <div class="hero-content">
            <span class="hero-badge">New Season 2026</span>
            <h1 class="hero-title">Discover the Art of<br><span class="highlight">Premium Living</span></h1>
            <p class="hero-subtitle">Curated collections of luxury essentials designed for those who appreciate the finer things in life.</p>
            <div class="hero-cta">
                <a href="#shop" class="btn btn-primary">Explore Collection <i class="fas fa-arrow-right"></i></a>
                <a href="#about" class="btn btn-outline">Our Story</a>
            </div>
            <div class="hero-stats">
                <div class="stat">
                    <span class="stat-number" data-count="12">0</span><span class="stat-suffix">K+</span>
                    <span class="stat-label">Happy Customers</span>
                </div>
                <div class="stat">
                    <span class="stat-number" data-count="500">0</span><span class="stat-suffix">+</span>
                    <span class="stat-label">Premium Products</span>
                </div>
                <div class="stat">
                    <span class="stat-number" data-count="98">0</span><span class="stat-suffix">%</span>
                    <span class="stat-label">Satisfaction Rate</span>
                </div>
            </div>
        </div>
        <div class="scroll-indicator">
            <span>Scroll</span>
            <div class="scroll-line"></div>
        </div>
    </section>

    <!-- ===================== BRAND MARQUEE ===================== -->
    <section class="brand-marquee">
        <div class="marquee-track">
            <div class="marquee-content">
                <span class="brand-name">GUCCI</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">PRADA</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">HERMÈS</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">CHANEL</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">DIOR</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">VERSACE</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">BURBERRY</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">GUCCI</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">PRADA</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">HERMÈS</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">CHANEL</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">DIOR</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">VERSACE</span>
                <span class="brand-dot">●</span>
                <span class="brand-name">BURBERRY</span>
                <span class="brand-dot">●</span>
            </div>
        </div>
    </section>

    <!-- ===================== CATEGORIES ===================== -->
    <section class="categories" id="collections">
        <div class="container">
            <div class="section-header">
                <span class="section-tag">Browse</span>
                <h2 class="section-title">Shop by Category</h2>
                <p class="section-desc">Find exactly what you're looking for across our curated collections</p>
            </div>
            <div class="category-grid">
                <div class="category-card category-large">
                    <img src="https://images.unsplash.com/photo-1483985988355-763728e1935b?w=800&q=80" alt="Fashion" class="category-img">
                    <div class="category-overlay">
                        <h3>Fashion</h3>
                        <p>120+ Products</p>
                        <a href="#" class="category-link">Shop Now <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>
                <div class="category-card">
                    <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?w=600&q=80" alt="Accessories" class="category-img">
                    <div class="category-overlay">
                        <h3>Accessories</h3>
                        <p>85+ Products</p>
                        <a href="#" class="category-link">Shop Now <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>
                <div class="category-card">
                    <img src="https://images.unsplash.com/photo-1616486338812-3dadae4b4ace?w=600&q=80" alt="Home & Living" class="category-img">
                    <div class="category-overlay">
                        <h3>Home & Living</h3>
                        <p>95+ Products</p>
                        <a href="#" class="category-link">Shop Now <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>
                <div class="category-card">
                    <img src="https://images.unsplash.com/photo-1585386959984-a4155224a1ad?w=600&q=80" alt="Fragrances" class="category-img">
                    <div class="category-overlay">
                        <h3>Fragrances</h3>
                        <p>60+ Products</p>
                        <a href="#" class="category-link">Shop Now <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>
                <div class="category-card category-wide">
                    <img src="https://images.unsplash.com/photo-1491553895911-0055eca6402d?w=800&q=80" alt="Footwear" class="category-img">
                    <div class="category-overlay">
                        <h3>Footwear</h3>
                        <p>75+ Products</p>
                        <a href="#" class="category-link">Shop Now <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ===================== PRODUCTS ===================== -->
    <section class="products" id="shop">
        <div class="container">
            <div class="section-header">
                <span class="section-tag">Trending</span>
                <h2 class="section-title">Featured Products</h2>
                <p class="section-desc">Hand-picked selections from our latest arrivals</p>
            </div>
            <div class="product-filters">
                <button class="filter-btn active" data-filter="all">All</button>
                <button class="filter-btn" data-filter="fashion">Fashion</button>
                <button class="filter-btn" data-filter="accessories">Accessories</button>
                <button class="filter-btn" data-filter="shoes">Footwear</button>
                <button class="filter-btn" data-filter="home">Home</button>
            </div>
            <div class="product-grid">
                <!-- Product 1 -->
                <div class="product-card" data-category="fashion">
                    <div class="product-img-wrap">
                        <span class="product-badge badge-new">New</span>
                        <img src="https://images.unsplash.com/photo-1594938298603-c8148c4dae35?w=500&q=80" alt="Premium Wool Coat" class="product-img">
                        <div class="product-actions">
                            <button class="product-action-btn" title="Quick View"><i class="fas fa-eye"></i></button>
                            <button class="product-action-btn" title="Add to Wishlist"><i class="fas fa-heart"></i></button>
                            <button class="product-action-btn add-to-cart" title="Add to Cart"><i class="fas fa-shopping-bag"></i></button>
                        </div>
                    </div>
                    <div class="product-info">
                        <span class="product-category">Fashion</span>
                        <h3 class="product-name">Premium Wool Overcoat</h3>
                        <div class="product-rating">
                            <div class="stars">
                                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star-half-alt"></i>
                            </div>
                            <span>(128)</span>
                        </div>
                        <div class="product-price">
                            <span class="current-price">$299.00</span>
                            <span class="original-price">$399.00</span>
                        </div>
                    </div>
                </div>

                <!-- Product 2 -->
                <div class="product-card" data-category="accessories">
                    <div class="product-img-wrap">
                        <span class="product-badge badge-sale">-30%</span>
                        <img src="https://images.unsplash.com/photo-1524592094714-0f0654e20314?w=500&q=80" alt="Luxury Watch" class="product-img">
                        <div class="product-actions">
                            <button class="product-action-btn" title="Quick View"><i class="fas fa-eye"></i></button>
                            <button class="product-action-btn" title="Add to Wishlist"><i class="fas fa-heart"></i></button>
                            <button class="product-action-btn add-to-cart" title="Add to Cart"><i class="fas fa-shopping-bag"></i></button>
                        </div>
                    </div>
                    <div class="product-info">
                        <span class="product-category">Accessories</span>
                        <h3 class="product-name">Classic Chronograph Watch</h3>
                        <div class="product-rating">
                            <div class="stars">
                                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
                            </div>
                            <span>(256)</span>
                        </div>
                        <div class="product-price">
                            <span class="current-price">$549.00</span>
                            <span class="original-price">$785.00</span>
                        </div>
                    </div>
                </div>

                <!-- Product 3 -->
                <div class="product-card" data-category="shoes">
                    <div class="product-img-wrap">
                        <img src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?w=500&q=80" alt="Designer Sneakers" class="product-img">
                        <div class="product-actions">
                            <button class="product-action-btn" title="Quick View"><i class="fas fa-eye"></i></button>
                            <button class="product-action-btn" title="Add to Wishlist"><i class="fas fa-heart"></i></button>
                            <button class="product-action-btn add-to-cart" title="Add to Cart"><i class="fas fa-shopping-bag"></i></button>
                        </div>
                    </div>
                    <div class="product-info">
                        <span class="product-category">Footwear</span>
                        <h3 class="product-name">Designer Sport Sneakers</h3>
                        <div class="product-rating">
                            <div class="stars">
                                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="far fa-star"></i>
                            </div>
                            <span>(92)</span>
                        </div>
                        <div class="product-price">
                            <span class="current-price">$189.00</span>
                        </div>
                    </div>
                </div>

                <!-- Product 4 -->
                <div class="product-card" data-category="accessories">
                    <div class="product-img-wrap">
                        <span class="product-badge badge-hot">Hot</span>
                        <img src="https://images.unsplash.com/photo-1584917865442-de89df76afd3?w=500&q=80" alt="Leather Handbag" class="product-img">
                        <div class="product-actions">
                            <button class="product-action-btn" title="Quick View"><i class="fas fa-eye"></i></button>
                            <button class="product-action-btn" title="Add to Wishlist"><i class="fas fa-heart"></i></button>
                            <button class="product-action-btn add-to-cart" title="Add to Cart"><i class="fas fa-shopping-bag"></i></button>
                        </div>
                    </div>
                    <div class="product-info">
                        <span class="product-category">Accessories</span>
                        <h3 class="product-name">Italian Leather Handbag</h3>
                        <div class="product-rating">
                            <div class="stars">
                                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star-half-alt"></i>
                            </div>
                            <span>(174)</span>
                        </div>
                        <div class="product-price">
                            <span class="current-price">$425.00</span>
                            <span class="original-price">$550.00</span>
                        </div>
                    </div>
                </div>

                <!-- Product 5 -->
                <div class="product-card" data-category="home">
                    <div class="product-img-wrap">
                        <img src="https://images.unsplash.com/photo-1602028915047-37269d1a73f7?w=500&q=80" alt="Scented Candle" class="product-img">
                        <div class="product-actions">
                            <button class="product-action-btn" title="Quick View"><i class="fas fa-eye"></i></button>
                            <button class="product-action-btn" title="Add to Wishlist"><i class="fas fa-heart"></i></button>
                            <button class="product-action-btn add-to-cart" title="Add to Cart"><i class="fas fa-shopping-bag"></i></button>
                        </div>
                    </div>
                    <div class="product-info">
                        <span class="product-category">Home</span>
                        <h3 class="product-name">Artisan Scented Candle Set</h3>
                        <div class="product-rating">
                            <div class="stars">
                                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
                            </div>
                            <span>(312)</span>
                        </div>
                        <div class="product-price">
                            <span class="current-price">$79.00</span>
                        </div>
                    </div>
                </div>

                <!-- Product 6 -->
                <div class="product-card" data-category="fashion">
                    <div class="product-img-wrap">
                        <span class="product-badge badge-new">New</span>
                        <img src="https://images.unsplash.com/photo-1591047139829-d91aecb6caea?w=500&q=80" alt="Designer Jacket" class="product-img">
                        <div class="product-actions">
                            <button class="product-action-btn" title="Quick View"><i class="fas fa-eye"></i></button>
                            <button class="product-action-btn" title="Add to Wishlist"><i class="fas fa-heart"></i></button>
                            <button class="product-action-btn add-to-cart" title="Add to Cart"><i class="fas fa-shopping-bag"></i></button>
                        </div>
                    </div>
                    <div class="product-info">
                        <span class="product-category">Fashion</span>
                        <h3 class="product-name">Premium Puffer Jacket</h3>
                        <div class="product-rating">
                            <div class="stars">
                                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star-half-alt"></i>
                            </div>
                            <span>(89)</span>
                        </div>
                        <div class="product-price">
                            <span class="current-price">$349.00</span>
                        </div>
                    </div>
                </div>

                <!-- Product 7 -->
                <div class="product-card" data-category="accessories">
                    <div class="product-img-wrap">
                        <img src="https://images.unsplash.com/photo-1572635196237-14b3f281503f?w=500&q=80" alt="Sunglasses" class="product-img">
                        <div class="product-actions">
                            <button class="product-action-btn" title="Quick View"><i class="fas fa-eye"></i></button>
                            <button class="product-action-btn" title="Add to Wishlist"><i class="fas fa-heart"></i></button>
                            <button class="product-action-btn add-to-cart" title="Add to Cart"><i class="fas fa-shopping-bag"></i></button>
                        </div>
                    </div>
                    <div class="product-info">
                        <span class="product-category">Accessories</span>
                        <h3 class="product-name">Aviator Sunglasses</h3>
                        <div class="product-rating">
                            <div class="stars">
                                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="far fa-star"></i>
                            </div>
                            <span>(67)</span>
                        </div>
                        <div class="product-price">
                            <span class="current-price">$159.00</span>
                            <span class="original-price">$210.00</span>
                        </div>
                    </div>
                </div>

                <!-- Product 8 -->
                <div class="product-card" data-category="shoes">
                    <div class="product-img-wrap">
                        <span class="product-badge badge-sale">-25%</span>
                        <img src="https://images.unsplash.com/photo-1608231387042-66d1773070a5?w=500&q=80" alt="Leather Boots" class="product-img">
                        <div class="product-actions">
                            <button class="product-action-btn" title="Quick View"><i class="fas fa-eye"></i></button>
                            <button class="product-action-btn" title="Add to Wishlist"><i class="fas fa-heart"></i></button>
                            <button class="product-action-btn add-to-cart" title="Add to Cart"><i class="fas fa-shopping-bag"></i></button>
                        </div>
                    </div>
                    <div class="product-info">
                        <span class="product-category">Footwear</span>
                        <h3 class="product-name">Handcrafted Leather Boots</h3>
                        <div class="product-rating">
                            <div class="stars">
                                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
                            </div>
                            <span>(203)</span>
                        </div>
                        <div class="product-price">
                            <span class="current-price">$275.00</span>
                            <span class="original-price">$365.00</span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="products-cta">
                <a href="#" class="btn btn-primary">View All Products <i class="fas fa-arrow-right"></i></a>
            </div>
        </div>
    </section>

    <!-- ===================== PROMO BANNER ===================== -->
    <section class="promo-banner">
        <div class="promo-bg">
            <img src="https://images.unsplash.com/photo-1445205170230-053b83016050?w=1920&q=80" alt="Sale Banner" class="promo-bg-img">
            <div class="promo-overlay"></div>
        </div>
        <div class="promo-content">
            <span class="promo-tag">Limited Time Offer</span>
            <h2 class="promo-title">Winter Sale<br>Up to <span class="promo-highlight">50% Off</span></h2>
            <p class="promo-text">Exclusive deals on premium winter essentials. Don't miss out on the season's best prices.</p>
            <div class="countdown" id="countdown">
                <div class="countdown-item">
                    <span class="countdown-num" id="days">05</span>
                    <span class="countdown-label">Days</span>
                </div>
                <div class="countdown-item">
                    <span class="countdown-num" id="hours">12</span>
                    <span class="countdown-label">Hours</span>
                </div>
                <div class="countdown-item">
                    <span class="countdown-num" id="minutes">38</span>
                    <span class="countdown-label">Min</span>
                </div>
                <div class="countdown-item">
                    <span class="countdown-num" id="seconds">45</span>
                    <span class="countdown-label">Sec</span>
                </div>
            </div>
            <a href="#" class="btn btn-primary btn-lg">Shop the Sale <i class="fas fa-arrow-right"></i></a>
        </div>
    </section>

    <!-- ===================== FEATURES ===================== -->
    <section class="features" id="about">
        <div class="container">
            <div class="section-header">
                <span class="section-tag">Why Us</span>
                <h2 class="section-title">The LUXORA Experience</h2>
                <p class="section-desc">What sets us apart from the rest</p>
            </div>
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-gem"></i>
                    </div>
                    <h3>Premium Quality</h3>
                    <p>Every product is carefully curated and quality-checked to meet our exacting standards.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-shipping-fast"></i>
                    </div>
                    <h3>Express Delivery</h3>
                    <p>Free express shipping worldwide on all orders over $99 with real-time tracking.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-undo-alt"></i>
                    </div>
                    <h3>Easy Returns</h3>
                    <p>30-day hassle-free returns with prepaid shipping labels on every order.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-headset"></i>
                    </div>
                    <h3>24/7 Support</h3>
                    <p>Our dedicated team is available around the clock to assist you with anything.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>Secure Payments</h3>
                    <p>Your transactions are protected with bank-level encryption and security.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-award"></i>
                    </div>
                    <h3>Authenticity Guaranteed</h3>
                    <p>100% genuine products sourced directly from authorized distributors.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- ===================== TESTIMONIALS ===================== -->
    <section class="testimonials" id="testimonials">
        <div class="container">
            <div class="section-header">
                <span class="section-tag">Testimonials</span>
                <h2 class="section-title">What Our Customers Say</h2>
                <p class="section-desc">Real reviews from verified buyers</p>
            </div>
            <div class="testimonial-slider">
                <div class="testimonial-track" id="testimonialTrack">
                    <div class="testimonial-card">
                        <div class="testimonial-stars">
                            <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
                        </div>
                        <p class="testimonial-text">"The quality exceeded my expectations. The wool overcoat I ordered is absolutely stunning and fits perfectly. LUXORA has become my go-to for premium fashion."</p>
                        <div class="testimonial-author">
                            <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?w=100&q=80" alt="Sarah Johnson" class="author-img">
                            <div>
                                <h4>Sarah Johnson</h4>
                                <span>Verified Buyer</span>
                            </div>
                        </div>
                    </div>
                    <div class="testimonial-card">
                        <div class="testimonial-stars">
                            <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
                        </div>
                        <p class="testimonial-text">"Incredible customer service and fast delivery. I received my order within 2 days with beautiful packaging. The watch I bought is a true masterpiece. Highly recommended!"</p>
                        <div class="testimonial-author">
                            <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=100&q=80" alt="Michael Chen" class="author-img">
                            <div>
                                <h4>Michael Chen</h4>
                                <span>Verified Buyer</span>
                            </div>
                        </div>
                    </div>
                    <div class="testimonial-card">
                        <div class="testimonial-stars">
                            <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star-half-alt"></i>
                        </div>
                        <p class="testimonial-text">"I've been shopping with LUXORA for over a year now. The consistency in quality and the curated selection makes it so easy to find exactly what I need. Love it!"</p>
                        <div class="testimonial-author">
                            <img src="https://images.unsplash.com/photo-1438761681033-6461ffad8d80?w=100&q=80" alt="Emma Williams" class="author-img">
                            <div>
                                <h4>Emma Williams</h4>
                                <span>Verified Buyer</span>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="testimonial-nav">
                    <button class="testimonial-btn" id="prevTestimonial"><i class="fas fa-chevron-left"></i></button>
                    <div class="testimonial-dots" id="testimonialDots">
                        <span class="dot active"></span>
                        <span class="dot"></span>
                        <span class="dot"></span>
                    </div>
                    <button class="testimonial-btn" id="nextTestimonial"><i class="fas fa-chevron-right"></i></button>
                </div>
            </div>
        </div>
    </section>

    <!-- ===================== NEWSLETTER ===================== -->
    <section class="newsletter" id="contact">
        <div class="container">
            <div class="newsletter-flex">
                <div class="newsletter-content">
                    <span class="section-tag">Stay Connected</span>
                    <h2 class="newsletter-title">Join the LUXORA Family</h2>
                    <p>Subscribe and get 15% off your first order, plus exclusive access to new arrivals and special offers.</p>
                </div>
                <form class="newsletter-form" id="newsletterForm">
                    <div class="input-group">
                        <input type="email" placeholder="Enter your email address" required class="newsletter-input">
                        <button type="submit" class="btn btn-primary">Subscribe <i class="fas fa-paper-plane"></i></button>
                    </div>
                    <p class="newsletter-disclaimer"><i class="fas fa-lock"></i> We respect your privacy. Unsubscribe anytime.</p>
                </form>
            </div>
        </div>
    </section>

    <!-- ===================== INSTAGRAM FEED ===================== -->
    <section class="instagram-feed">
        <div class="section-header">
            <span class="section-tag">@LUXORA</span>
            <h2 class="section-title">Follow Us on Instagram</h2>
        </div>
        <div class="insta-grid">
            <a href="#" class="insta-item">
                <img src="https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?w=400&q=80" alt="Instagram post">
                <div class="insta-overlay"><i class="fab fa-instagram"></i></div>
            </a>
            <a href="#" class="insta-item">
                <img src="https://images.unsplash.com/photo-1558618666-fcd25c85f82e?w=400&q=80" alt="Instagram post">
                <div class="insta-overlay"><i class="fab fa-instagram"></i></div>
            </a>
            <a href="#" class="insta-item">
                <img src="https://images.unsplash.com/photo-1543163521-1bf539c55dd2?w=400&q=80" alt="Instagram post">
                <div class="insta-overlay"><i class="fab fa-instagram"></i></div>
            </a>
            <a href="#" class="insta-item">
                <img src="https://images.unsplash.com/photo-1548036328-c9fa89d128fa?w=400&q=80" alt="Instagram post">
                <div class="insta-overlay"><i class="fab fa-instagram"></i></div>
            </a>
            <a href="#" class="insta-item">
                <img src="https://images.unsplash.com/photo-1556906781-9a412961c28c?w=400&q=80" alt="Instagram post">
                <div class="insta-overlay"><i class="fab fa-instagram"></i></div>
            </a>
            <a href="#" class="insta-item">
                <img src="https://images.unsplash.com/photo-1560769629-975ec94e6a86?w=400&q=80" alt="Instagram post">
                <div class="insta-overlay"><i class="fab fa-instagram"></i></div>
            </a>
        </div>
    </section>

    <!-- ===================== FOOTER ===================== -->
    <footer class="footer">
        <div class="container">
            <div class="footer-grid">
                <div class="footer-col footer-brand">
                    <a href="#" class="footer-logo"><span class="logo-icon">◆</span> LUXORA</a>
                    <p>Your destination for premium lifestyle products. Curating excellence since 2020.</p>
                    <div class="footer-social">
                        <a href="#" class="social-link" aria-label="Facebook"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="social-link" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="social-link" aria-label="Twitter"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="social-link" aria-label="Pinterest"><i class="fab fa-pinterest-p"></i></a>
                        <a href="#" class="social-link" aria-label="YouTube"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div class="footer-col">
                    <h4>Quick Links</h4>
                    <ul>
                        <li><a href="#">New Arrivals</a></li>
                        <li><a href="#">Best Sellers</a></li>
                        <li><a href="#">Sale</a></li>
                        <li><a href="#">Gift Cards</a></li>
                        <li><a href="#">Our Story</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h4>Customer Care</h4>
                    <ul>
                        <li><a href="#">Help Center</a></li>
                        <li><a href="#">Shipping & Delivery</a></li>
                        <li><a href="#">Returns & Exchanges</a></li>
                        <li><a href="#">Size Guide</a></li>
                        <li><a href="#">Track Your Order</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h4>Contact Us</h4>
                    <ul class="contact-list">
                        <li><i class="fas fa-map-marker-alt"></i> 123 Fifth Avenue, New York, NY 10001</li>
                        <li><i class="fas fa-phone-alt"></i> +1 (555) 123-4567</li>
                        <li><i class="fas fa-envelope"></i> hello@luxora.com</li>
                        <li><i class="fas fa-clock"></i> Mon - Fri: 9AM - 6PM EST</li>
                    </ul>
                </div>
            </div>
            <div class="footer-bottom">
                <div class="footer-bottom-flex">
                    <p>&copy; 2026 LUXORA. All rights reserved.</p>
                    <div class="footer-links">
                        <a href="#">Privacy Policy</a>
                        <a href="#">Terms of Service</a>
                        <a href="#">Cookie Policy</a>
                    </div>
                    <div class="payment-methods">
                        <i class="fab fa-cc-visa"></i>
                        <i class="fab fa-cc-mastercard"></i>
                        <i class="fab fa-cc-amex"></i>
                        <i class="fab fa-cc-paypal"></i>
                        <i class="fab fa-cc-apple-pay"></i>
                    </div>
                </div>
            </div>
        </div>
    </footer>

    <!-- Back to Top -->
    <button class="back-to-top" id="backToTop" aria-label="Back to top">
        <i class="fas fa-chevron-up"></i>
    </button>

    <!-- Toast Notification -->
    <div class="toast" id="toast">
        <i class="fas fa-check-circle"></i>
        <span id="toastMessage">Item added to cart!</span>
    </div>

    <script src="script.js"></script>
</body>
</html>
```
script.js
```
/* ===================================================================
   LUXORA — Premium Lifestyle Store
   JavaScript — Interactivity & Animations
   =================================================================== */

document.addEventListener('DOMContentLoaded', () => {

    // ===================== HEADER SCROLL EFFECT =====================
    const header = document.getElementById('header');
    const announcementBar = document.querySelector('.announcement-bar');

    const handleScroll = () => {
        const scrollY = window.scrollY;
        if (scrollY > 60) {
            header.classList.add('scrolled');
            if (announcementBar) announcementBar.style.transform = 'translateY(-100%)';
            header.style.paddingTop = '0';
        } else {
            header.classList.remove('scrolled');
            if (announcementBar) announcementBar.style.transform = 'translateY(0)';
        }
    };

    window.addEventListener('scroll', handleScroll);
    handleScroll();

    // ===================== MOBILE NAVIGATION =====================
    const hamburger = document.getElementById('hamburger');
    const navLinks = document.getElementById('navLinks');

    if (hamburger && navLinks) {
        hamburger.addEventListener('click', () => {
            hamburger.classList.toggle('active');
            navLinks.classList.toggle('active');
            document.body.style.overflow = navLinks.classList.contains('active') ? 'hidden' : '';
        });

        // Close mobile nav when a link is clicked
        navLinks.querySelectorAll('.nav-link').forEach(link => {
            link.addEventListener('click', () => {
                hamburger.classList.remove('active');
                navLinks.classList.remove('active');
                document.body.style.overflow = '';
            });
        });
    }

    // ===================== ACTIVE NAV LINK =====================
    const sections = document.querySelectorAll('section[id]');
    const navLinkItems = document.querySelectorAll('.nav-link');

    const setActiveLink = () => {
        const scrollPos = window.scrollY + 150;
        sections.forEach(section => {
            const top = section.offsetTop;
            const height = section.offsetHeight;
            const id = section.getAttribute('id');
            if (scrollPos >= top && scrollPos < top + height) {
                navLinkItems.forEach(link => {
                    link.classList.remove('active');
                    if (link.getAttribute('href') === `#${id}`) {
                        link.classList.add('active');
                    }
                });
            }
        });
    };

    window.addEventListener('scroll', setActiveLink);

    // ===================== SEARCH OVERLAY =====================
    const searchBtn = document.getElementById('searchBtn');
    const searchOverlay = document.getElementById('searchOverlay');
    const searchClose = document.getElementById('searchClose');
    const searchInput = document.getElementById('searchInput');

    if (searchBtn && searchOverlay) {
        searchBtn.addEventListener('click', () => {
            searchOverlay.classList.toggle('active');
            if (searchOverlay.classList.contains('active') && searchInput) {
                setTimeout(() => searchInput.focus(), 300);
            }
        });

        if (searchClose) {
            searchClose.addEventListener('click', () => {
                searchOverlay.classList.remove('active');
            });
        }
    }

    // ===================== PRODUCT FILTER =====================
    const filterBtns = document.querySelectorAll('.filter-btn');
    const productCards = document.querySelectorAll('.product-card');

    filterBtns.forEach(btn => {
        btn.addEventListener('click', () => {
            filterBtns.forEach(b => b.classList.remove('active'));
            btn.classList.add('active');

            const filter = btn.dataset.filter;

            productCards.forEach((card, index) => {
                const category = card.dataset.category;

                if (filter === 'all' || category === filter) {
                    card.classList.remove('hidden');
                    card.style.animation = `fadeInUp 0.5s ease ${index * 0.08}s both`;
                } else {
                    card.classList.add('hidden');
                }
            });
        });
    });

    // ===================== ADD TO CART =====================
    const cartCountEl = document.getElementById('cartCount');
    let cartCount = 2;

    document.querySelectorAll('.add-to-cart').forEach(btn => {
        btn.addEventListener('click', (e) => {
            e.stopPropagation();
            cartCount++;
            if (cartCountEl) cartCountEl.textContent = cartCount;

            // Get product name for toast
            const card = btn.closest('.product-card');
            const productName = card ? card.querySelector('.product-name')?.textContent : 'Item';
            showToast(`${productName} added to cart!`);

            // Button animation
            btn.style.transform = 'scale(1.3)';
            btn.style.background = '#27ae60';
            btn.innerHTML = '<i class="fas fa-check"></i>';
            setTimeout(() => {
                btn.style.transform = '';
                btn.style.background = '';
                btn.innerHTML = '<i class="fas fa-shopping-bag"></i>';
            }, 1500);
        });
    });

    // ===================== TOAST NOTIFICATION =====================
    const toast = document.getElementById('toast');
    const toastMessage = document.getElementById('toastMessage');
    let toastTimeout;

    function showToast(message) {
        if (!toast || !toastMessage) return;
        toastMessage.textContent = message;
        toast.classList.add('show');
        clearTimeout(toastTimeout);
        toastTimeout = setTimeout(() => {
            toast.classList.remove('show');
        }, 3000);
    }

    // ===================== TESTIMONIAL SLIDER =====================
    const testimonialTrack = document.getElementById('testimonialTrack');
    const prevBtn = document.getElementById('prevTestimonial');
    const nextBtn = document.getElementById('nextTestimonial');
    const dots = document.querySelectorAll('.dot');
    let currentSlide = 0;
    const totalSlides = document.querySelectorAll('.testimonial-card').length;

    function goToSlide(index) {
        if (index < 0) index = totalSlides - 1;
        if (index >= totalSlides) index = 0;
        currentSlide = index;

        if (testimonialTrack) {
            testimonialTrack.style.transform = `translateX(-${currentSlide * 100}%)`;
        }

        dots.forEach((dot, i) => {
            dot.classList.toggle('active', i === currentSlide);
        });
    }

    if (prevBtn) prevBtn.addEventListener('click', () => goToSlide(currentSlide - 1));
    if (nextBtn) nextBtn.addEventListener('click', () => goToSlide(currentSlide + 1));

    dots.forEach((dot, i) => {
        dot.addEventListener('click', () => goToSlide(i));
    });

    // Auto-slide every 5 seconds
    let autoSlide = setInterval(() => goToSlide(currentSlide + 1), 5000);

    // Pause on hover
    const testimonialSlider = document.querySelector('.testimonial-slider');
    if (testimonialSlider) {
        testimonialSlider.addEventListener('mouseenter', () => clearInterval(autoSlide));
        testimonialSlider.addEventListener('mouseleave', () => {
            autoSlide = setInterval(() => goToSlide(currentSlide + 1), 5000);
        });
    }

    // ===================== COUNTDOWN TIMER =====================
    function updateCountdown() {
        const now = new Date();
        const target = new Date(now);
        target.setDate(target.getDate() + 5);
        target.setHours(23, 59, 59, 0);

        // Store the target in localStorage so it persists
        const storedTarget = localStorage.getItem('luxora_sale_end');
        let endDate;

        if (storedTarget) {
            endDate = new Date(storedTarget);
            if (endDate <= now) {
                endDate = target;
                localStorage.setItem('luxora_sale_end', target.toISOString());
            }
        } else {
            endDate = target;
            localStorage.setItem('luxora_sale_end', target.toISOString());
        }

        const diff = endDate - now;

        const days = Math.floor(diff / (1000 * 60 * 60 * 24));
        const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
        const seconds = Math.floor((diff % (1000 * 60)) / 1000);

        const daysEl = document.getElementById('days');
        const hoursEl = document.getElementById('hours');
        const minutesEl = document.getElementById('minutes');
        const secondsEl = document.getElementById('seconds');

        if (daysEl) daysEl.textContent = String(days).padStart(2, '0');
        if (hoursEl) hoursEl.textContent = String(hours).padStart(2, '0');
        if (minutesEl) minutesEl.textContent = String(minutes).padStart(2, '0');
        if (secondsEl) secondsEl.textContent = String(seconds).padStart(2, '0');
    }

    updateCountdown();
    setInterval(updateCountdown, 1000);

    // ===================== NUMBER COUNTER ANIMATION =====================
    const counters = document.querySelectorAll('.stat-number');
    let counterObserved = false;

    function animateCounters() {
        if (counterObserved) return;

        counters.forEach(counter => {
            const target = parseInt(counter.dataset.count);
            const duration = 2000;
            const step = target / (duration / 16);
            let current = 0;

            const updateCounter = () => {
                current += step;
                if (current < target) {
                    counter.textContent = Math.floor(current);
                    requestAnimationFrame(updateCounter);
                } else {
                    counter.textContent = target;
                }
            };

            updateCounter();
        });

        counterObserved = true;
    }

    // Trigger counter when hero stats are visible
    const statsObserver = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                animateCounters();
            }
        });
    }, { threshold: 0.5 });

    const heroStats = document.querySelector('.hero-stats');
    if (heroStats) statsObserver.observe(heroStats);

    // ===================== SCROLL REVEAL ANIMATIONS =====================
    const revealElements = document.querySelectorAll(
        '.category-card, .product-card, .feature-card, .testimonial-slider, .newsletter-flex, .footer-grid'
    );

    revealElements.forEach(el => el.classList.add('reveal'));

    const revealObserver = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                entry.target.classList.add('active');
                revealObserver.unobserve(entry.target);
            }
        });
    }, { threshold: 0.1, rootMargin: '0px 0px -50px 0px' });

    revealElements.forEach(el => revealObserver.observe(el));

    // ===================== BACK TO TOP BUTTON =====================
    const backToTop = document.getElementById('backToTop');

    window.addEventListener('scroll', () => {
        if (window.scrollY > 500) {
            backToTop?.classList.add('visible');
        } else {
            backToTop?.classList.remove('visible');
        }
    });

    if (backToTop) {
        backToTop.addEventListener('click', () => {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        });
    }

    // ===================== NEWSLETTER FORM =====================
    const newsletterForm = document.getElementById('newsletterForm');

    if (newsletterForm) {
        newsletterForm.addEventListener('submit', (e) => {
            e.preventDefault();
            const emailInput = newsletterForm.querySelector('.newsletter-input');
            if (emailInput && emailInput.value) {
                showToast('Successfully subscribed! Welcome to LUXORA 🎉');
                emailInput.value = '';
            }
        });
    }

    // ===================== SMOOTH SCROLL FOR NAV LINKS =====================
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function(e) {
            const targetId = this.getAttribute('href');
            if (targetId === '#') return;

            const targetEl = document.querySelector(targetId);
            if (targetEl) {
                e.preventDefault();
                targetEl.scrollIntoView({ behavior: 'smooth' });
            }
        });
    });

    // ===================== PARALLAX EFFECT ON SCROLL =====================
    const promoSection = document.querySelector('.promo-bg-img');

    if (promoSection) {
        window.addEventListener('scroll', () => {
            const rect = promoSection.getBoundingClientRect();
            if (rect.top < window.innerHeight && rect.bottom > 0) {
                const speed = 0.3;
                const yPos = -(rect.top * speed);
                promoSection.style.transform = `translateY(${yPos}px)`;
            }
        });
    }

    // ===================== IMAGE LAZY LOADING =====================
    const lazyImages = document.querySelectorAll('img[src]');

    if ('IntersectionObserver' in window) {
        const imageObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const img = entry.target;
                    img.style.opacity = '1';
                    imageObserver.unobserve(img);
                }
            });
        });

        lazyImages.forEach(img => {
            img.style.opacity = '0';
            img.style.transition = 'opacity 0.5s ease';
            imageObserver.observe(img);
        });
    }

    // ===================== PRODUCT CARD HOVER TILT =====================
    document.querySelectorAll('.product-card').forEach(card => {
        card.addEventListener('mousemove', (e) => {
            const rect = card.getBoundingClientRect();
            const x = e.clientX - rect.left;
            const y = e.clientY - rect.top;
            const centerX = rect.width / 2;
            const centerY = rect.height / 2;
            const rotateX = (y - centerY) / 30;
            const rotateY = (centerX - x) / 30;

            card.style.transform = `translateY(-8px) perspective(1000px) rotateX(${rotateX}deg) rotateY(${rotateY}deg)`;
        });

        card.addEventListener('mouseleave', () => {
            card.style.transform = '';
        });
    });

    console.log('%c🛍️ LUXORA — Premium Lifestyle Store', 'font-size: 18px; font-weight: bold; color: #c9a96e;');
    console.log('%cBuilt with CSS Flexbox | Responsive Design', 'font-size: 12px; color: #888;');
});
```
server.js
```
/**
 * Lightweight Zero-Dependency Local Static Server
 * Usage: node server.js [port]
 */

const http = require('http');
const fs = require('fs');
const path = require('path');

const PORT = parseInt(process.argv[2], 10) || 3000;
const PUBLIC_DIR = __dirname;

const MIME_TYPES = {
    '.html': 'text/html; charset=utf-8',
    '.css': 'text/css; charset=utf-8',
    '.js': 'application/javascript; charset=utf-8',
    '.json': 'application/json; charset=utf-8',
    '.png': 'image/png',
    '.jpg': 'image/jpeg',
    '.jpeg': 'image/jpeg',
    '.svg': 'image/svg+xml',
    '.ico': 'image/x-icon',
    '.md': 'text/markdown; charset=utf-8'
};

const server = http.createServer((req, res) => {
    let safeUrl = decodeURI(req.url.split('?')[0]);
    if (safeUrl === '/') safeUrl = '/index.html';

    const filePath = path.join(PUBLIC_DIR, safeUrl);

    // Prevent directory traversal
    if (!filePath.startsWith(PUBLIC_DIR)) {
        res.writeHead(403, { 'Content-Type': 'text/plain' });
        res.end('403 Forbidden');
        return;
    }

    fs.stat(filePath, (err, stats) => {
        if (err || !stats.isFile()) {
            res.writeHead(404, { 'Content-Type': 'text/plain' });
            res.end('404 Not Found');
            return;
        }

        const ext = path.extname(filePath).toLowerCase();
        const contentType = MIME_TYPES[ext] || 'application/octet-stream';

        res.writeHead(200, {
            'Content-Type': contentType,
            'Cache-Control': 'no-cache'
        });

        const stream = fs.createReadStream(filePath);
        stream.pipe(res);
    });
});

server.listen(PORT, '127.0.0.1', () => {
    console.log(`=======================================================`);
    console.log(` LUMINA TECH Commercial Flexbox Website is Live!`);
    console.log(` URL: http://127.0.0.1:${PORT}`);
    console.log(` Root Directory: ${PUBLIC_DIR}`);
    console.log(` Press Ctrl+C to terminate`);
    console.log(`=======================================================`);
});
```
style.css
```
/* ===================================================================
   LUXORA — Premium Lifestyle Store
   CSS Flexbox Responsive Layout
   =================================================================== */

/* ===================== CSS CUSTOM PROPERTIES ===================== */
:root {
    /* Colors */
    --primary: #1a1a2e;
    --primary-light: #16213e;
    --accent: #c9a96e;
    --accent-hover: #b8923f;
    --accent-light: rgba(201, 169, 110, 0.1);
    --white: #ffffff;
    --off-white: #f8f7f4;
    --light-gray: #f0eeeb;
    --gray: #9e9e9e;
    --dark-gray: #555;
    --text: #2c2c2c;
    --text-light: #6b6b6b;
    --danger: #e74c3c;
    --success: #27ae60;

    /* Typography */
    --font-heading: 'Playfair Display', Georgia, serif;
    --font-body: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;

    /* Spacing */
    --section-padding: 100px 0;
    --container-width: 1280px;
    --gap: 24px;

    /* Transitions */
    --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    --transition-slow: all 0.6s cubic-bezier(0.4, 0, 0.2, 1);

    /* Shadows */
    --shadow-sm: 0 2px 8px rgba(0, 0, 0, 0.06);
    --shadow-md: 0 8px 30px rgba(0, 0, 0, 0.08);
    --shadow-lg: 0 20px 60px rgba(0, 0, 0, 0.12);
    --shadow-xl: 0 30px 80px rgba(0, 0, 0, 0.18);

    /* Border Radius */
    --radius-sm: 8px;
    --radius-md: 12px;
    --radius-lg: 20px;
    --radius-full: 50%;
}

/* ===================== RESET & BASE ===================== */
*,
*::before,
*::after {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    scroll-padding-top: 80px;
    font-size: 16px;
}

body {
    font-family: var(--font-body);
    color: var(--text);
    background: var(--white);
    line-height: 1.7;
    overflow-x: hidden;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

a {
    text-decoration: none;
    color: inherit;
    transition: var(--transition);
}

img {
    max-width: 100%;
    display: block;
}

ul { list-style: none; }

button {
    border: none;
    background: none;
    cursor: pointer;
    font-family: inherit;
    transition: var(--transition);
}

.container {
    max-width: var(--container-width);
    margin: 0 auto;
    padding: 0 24px;
}

/* ===================== SECTION HEADERS ===================== */
.section-header {
    text-align: center;
    margin-bottom: 60px;
}

.section-tag {
    display: inline-block;
    font-size: 0.75rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 3px;
    color: var(--accent);
    margin-bottom: 12px;
    position: relative;
    padding: 0 20px;
}

.section-tag::before,
.section-tag::after {
    content: '';
    position: absolute;
    top: 50%;
    width: 30px;
    height: 1px;
    background: var(--accent);
}

.section-tag::before { left: -20px; }
.section-tag::after { right: -20px; }

.section-title {
    font-family: var(--font-heading);
    font-size: clamp(2rem, 4vw, 3rem);
    font-weight: 700;
    color: var(--primary);
    margin-bottom: 16px;
    line-height: 1.2;
}

.section-desc {
    font-size: 1.05rem;
    color: var(--text-light);
    max-width: 540px;
    margin: 0 auto;
}

/* ===================== BUTTONS ===================== */
.btn {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    padding: 14px 32px;
    font-size: 0.95rem;
    font-weight: 600;
    border-radius: 50px;
    transition: var(--transition);
    cursor: pointer;
    border: 2px solid transparent;
    letter-spacing: 0.5px;
}

.btn-primary {
    background: var(--accent);
    color: var(--white);
    border-color: var(--accent);
}

.btn-primary:hover {
    background: var(--accent-hover);
    border-color: var(--accent-hover);
    transform: translateY(-2px);
    box-shadow: 0 10px 30px rgba(201, 169, 110, 0.35);
}

.btn-outline {
    background: transparent;
    color: var(--white);
    border-color: rgba(255, 255, 255, 0.5);
}

.btn-outline:hover {
    background: var(--white);
    color: var(--primary);
    border-color: var(--white);
    transform: translateY(-2px);
}

.btn-lg {
    padding: 18px 42px;
    font-size: 1.05rem;
}

/* ===================== ANNOUNCEMENT BAR ===================== */
.announcement-bar {
    background: var(--primary);
    color: var(--white);
    text-align: center;
    padding: 10px 20px;
    font-size: 0.85rem;
    letter-spacing: 0.5px;
}

.announcement-bar a {
    color: var(--accent);
    font-weight: 600;
    text-decoration: underline;
    text-underline-offset: 3px;
}

.announcement-bar a:hover {
    color: var(--white);
}

.announcement-bar i {
    margin-right: 8px;
}

/* ===================== HEADER / NAVBAR (FLEXBOX) ===================== */
.header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 1000;
    transition: var(--transition);
    padding-top: 38px; /* announcement bar height */
}

.header.scrolled {
    background: rgba(255, 255, 255, 0.97);
    backdrop-filter: blur(20px);
    box-shadow: var(--shadow-sm);
    padding-top: 0;
}

.header.scrolled .nav-link { color: var(--text); }
.header.scrolled .nav-link:hover,
.header.scrolled .nav-link.active { color: var(--accent); }
.header.scrolled .logo { color: var(--primary); }
.header.scrolled .nav-icon-btn { color: var(--text); }

.navbar {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    justify-content: space-between;
    max-width: var(--container-width);
    margin: 0 auto;
    padding: 16px 24px;
}

.logo {
    font-family: var(--font-heading);
    font-size: 1.75rem;
    font-weight: 700;
    color: var(--white);
    letter-spacing: 3px;
    /* Flexbox for logo icon + text */
    display: flex;
    align-items: center;
    gap: 4px;
}

.logo-icon {
    color: var(--accent);
    font-size: 1.2rem;
}

.nav-links {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    gap: 36px;
}

.nav-link {
    font-size: 0.9rem;
    font-weight: 500;
    color: rgba(255, 255, 255, 0.85);
    position: relative;
    letter-spacing: 0.3px;
}

.nav-link::after {
    content: '';
    position: absolute;
    bottom: -4px;
    left: 0;
    width: 0;
    height: 2px;
    background: var(--accent);
    transition: var(--transition);
}

.nav-link:hover::after,
.nav-link.active::after { width: 100%; }

.nav-link:hover,
.nav-link.active { color: var(--white); }

.nav-actions {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    gap: 8px;
}

.nav-icon-btn {
    width: 42px;
    height: 42px;
    /* Flexbox centering */
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: var(--radius-full);
    color: rgba(255, 255, 255, 0.85);
    font-size: 1.05rem;
    position: relative;
}

.nav-icon-btn:hover {
    background: rgba(255, 255, 255, 0.1);
    color: var(--white);
}

.header.scrolled .nav-icon-btn:hover {
    background: var(--light-gray);
    color: var(--accent);
}

.badge {
    position: absolute;
    top: 2px;
    right: 2px;
    width: 18px;
    height: 18px;
    background: var(--accent);
    color: var(--white);
    font-size: 0.65rem;
    font-weight: 700;
    border-radius: var(--radius-full);
    /* Flexbox centering */
    display: flex;
    align-items: center;
    justify-content: center;
}

.hamburger {
    display: none;
    flex-direction: column;
    gap: 5px;
    padding: 8px;
}

.hamburger span {
    width: 24px;
    height: 2px;
    background: var(--white);
    transition: var(--transition);
    border-radius: 2px;
}

.header.scrolled .hamburger span { background: var(--text); }

.hamburger.active span:nth-child(1) { transform: rotate(45deg) translate(5px, 5px); }
.hamburger.active span:nth-child(2) { opacity: 0; }
.hamburger.active span:nth-child(3) { transform: rotate(-45deg) translate(5px, -5px); }

/* Search Overlay */
.search-overlay {
    position: absolute;
    top: 100%;
    left: 0;
    width: 100%;
    background: var(--white);
    padding: 0;
    max-height: 0;
    overflow: hidden;
    transition: var(--transition);
    box-shadow: var(--shadow-md);
}

.search-overlay.active {
    max-height: 100px;
    padding: 20px 0;
}

.search-container {
    max-width: var(--container-width);
    margin: 0 auto;
    padding: 0 24px;
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    gap: 16px;
}

.search-input {
    flex: 1;
    border: none;
    outline: none;
    font-size: 1.1rem;
    font-family: inherit;
    color: var(--text);
    background: transparent;
}

.search-close {
    font-size: 1.2rem;
    color: var(--gray);
}

.search-close:hover { color: var(--text); }

/* ===================== HERO SECTION ===================== */
.hero {
    position: relative;
    min-height: 100vh;
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
}

.hero-bg {
    position: absolute;
    inset: 0;
    z-index: 0;
}

.hero-bg-img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    animation: heroZoom 20s ease-in-out infinite alternate;
}

@keyframes heroZoom {
    from { transform: scale(1); }
    to { transform: scale(1.08); }
}

.hero-overlay {
    position: absolute;
    inset: 0;
    background: linear-gradient(
        135deg,
        rgba(26, 26, 46, 0.85) 0%,
        rgba(22, 33, 62, 0.65) 50%,
        rgba(26, 26, 46, 0.75) 100%
    );
}

.hero-content {
    position: relative;
    z-index: 2;
    text-align: center;
    color: var(--white);
    padding: 40px 24px;
    max-width: 800px;
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-direction: column;
    align-items: center;
}

.hero-badge {
    display: inline-block;
    padding: 8px 24px;
    border: 1px solid rgba(201, 169, 110, 0.5);
    border-radius: 50px;
    font-size: 0.8rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 3px;
    color: var(--accent);
    margin-bottom: 28px;
    animation: fadeInUp 0.8s ease-out;
}

.hero-title {
    font-family: var(--font-heading);
    font-size: clamp(2.5rem, 6vw, 4.5rem);
    font-weight: 700;
    line-height: 1.15;
    margin-bottom: 24px;
    animation: fadeInUp 0.8s ease-out 0.2s both;
}

.highlight {
    color: var(--accent);
    font-style: italic;
}

.hero-subtitle {
    font-size: clamp(1rem, 2vw, 1.2rem);
    color: rgba(255, 255, 255, 0.8);
    max-width: 560px;
    margin-bottom: 40px;
    line-height: 1.8;
    animation: fadeInUp 0.8s ease-out 0.4s both;
}

.hero-cta {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    gap: 16px;
    flex-wrap: wrap;
    justify-content: center;
    margin-bottom: 60px;
    animation: fadeInUp 0.8s ease-out 0.6s both;
}

.hero-stats {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    gap: 50px;
    animation: fadeInUp 0.8s ease-out 0.8s both;
}

.stat {
    text-align: center;
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-direction: column;
    align-items: center;
}

.stat-number {
    font-family: var(--font-heading);
    font-size: 2.2rem;
    font-weight: 700;
    color: var(--accent);
}

.stat-suffix {
    font-family: var(--font-heading);
    font-size: 1.5rem;
    font-weight: 600;
    color: var(--accent);
}

.stat-label {
    font-size: 0.8rem;
    color: rgba(255, 255, 255, 0.6);
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-top: 4px;
}

/* Scroll Indicator */
.scroll-indicator {
    position: absolute;
    bottom: 30px;
    left: 50%;
    transform: translateX(-50%);
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 8px;
    color: rgba(255, 255, 255, 0.5);
    font-size: 0.7rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    animation: fadeInUp 0.8s ease-out 1s both;
}

.scroll-line {
    width: 1px;
    height: 40px;
    background: linear-gradient(to bottom, var(--accent), transparent);
    animation: scrollBounce 2s ease-in-out infinite;
}

@keyframes scrollBounce {
    0%, 100% { transform: scaleY(1); opacity: 1; }
    50% { transform: scaleY(0.5); opacity: 0.5; }
}

/* ===================== BRAND MARQUEE ===================== */
.brand-marquee {
    background: var(--off-white);
    padding: 28px 0;
    overflow: hidden;
}

.marquee-track {
    overflow: hidden;
    white-space: nowrap;
}

.marquee-content {
    display: inline-flex;
    align-items: center;
    gap: 40px;
    animation: marqueeScroll 30s linear infinite;
}

.brand-name {
    font-family: var(--font-heading);
    font-size: 1.3rem;
    font-weight: 600;
    color: var(--gray);
    letter-spacing: 4px;
}

.brand-dot {
    color: var(--accent);
    font-size: 0.5rem;
}

@keyframes marqueeScroll {
    from { transform: translateX(0); }
    to { transform: translateX(-50%); }
}

/* ===================== CATEGORIES (FLEXBOX GRID) ===================== */
.categories {
    padding: var(--section-padding);
    background: var(--white);
}

.category-grid {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-wrap: wrap;
    gap: var(--gap);
}

.category-card {
    position: relative;
    border-radius: var(--radius-lg);
    overflow: hidden;
    flex: 1 1 calc(33.333% - var(--gap));
    min-height: 280px;
    cursor: pointer;
}

.category-card.category-large {
    flex: 1 1 calc(50% - var(--gap));
    min-height: 380px;
}

.category-card.category-wide {
    flex: 1 1 calc(50% - var(--gap));
    min-height: 300px;
}

.category-img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: var(--transition-slow);
}

.category-card:hover .category-img {
    transform: scale(1.1);
}

.category-overlay {
    position: absolute;
    inset: 0;
    background: linear-gradient(to top, rgba(26, 26, 46, 0.85) 0%, transparent 60%);
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    padding: 30px;
    color: var(--white);
}

.category-overlay h3 {
    font-family: var(--font-heading);
    font-size: 1.5rem;
    font-weight: 700;
    margin-bottom: 4px;
}

.category-overlay p {
    font-size: 0.85rem;
    color: rgba(255, 255, 255, 0.7);
    margin-bottom: 12px;
}

.category-link {
    font-size: 0.85rem;
    font-weight: 600;
    color: var(--accent);
    /* ★ FLEXBOX ★ */
    display: flex;
    align-items: center;
    gap: 8px;
    transform: translateX(0);
    transition: var(--transition);
}

.category-card:hover .category-link {
    transform: translateX(5px);
}

/* ===================== PRODUCTS (FLEXBOX GRID) ===================== */
.products {
    padding: var(--section-padding);
    background: var(--off-white);
}

.product-filters {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    justify-content: center;
    gap: 12px;
    margin-bottom: 48px;
    flex-wrap: wrap;
}

.filter-btn {
    padding: 10px 28px;
    font-size: 0.85rem;
    font-weight: 600;
    border: 2px solid var(--light-gray);
    border-radius: 50px;
    color: var(--text-light);
    background: var(--white);
    transition: var(--transition);
}

.filter-btn:hover,
.filter-btn.active {
    border-color: var(--accent);
    color: var(--accent);
    background: var(--accent-light);
}

.product-grid {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-wrap: wrap;
    gap: var(--gap);
}

.product-card {
    flex: 1 1 calc(25% - var(--gap));
    min-width: 240px;
    background: var(--white);
    border-radius: var(--radius-md);
    overflow: hidden;
    transition: var(--transition);
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-direction: column;
}

.product-card:hover {
    transform: translateY(-8px);
    box-shadow: var(--shadow-lg);
}

.product-card.hidden {
    display: none;
}

.product-img-wrap {
    position: relative;
    overflow: hidden;
    aspect-ratio: 3/4;
    background: var(--light-gray);
}

.product-badge {
    position: absolute;
    top: 14px;
    left: 14px;
    padding: 5px 14px;
    font-size: 0.7rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 1px;
    border-radius: 50px;
    z-index: 2;
}

.badge-new { background: var(--primary); color: var(--white); }
.badge-sale { background: var(--danger); color: var(--white); }
.badge-hot { background: var(--accent); color: var(--white); }

.product-img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: var(--transition-slow);
}

.product-card:hover .product-img {
    transform: scale(1.08);
}

.product-actions {
    position: absolute;
    right: 14px;
    top: 14px;
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-direction: column;
    gap: 8px;
    transform: translateX(60px);
    opacity: 0;
    transition: var(--transition);
}

.product-card:hover .product-actions {
    transform: translateX(0);
    opacity: 1;
}

.product-action-btn {
    width: 40px;
    height: 40px;
    background: var(--white);
    border-radius: var(--radius-full);
    /* ★ FLEXBOX centering ★ */
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.9rem;
    color: var(--text);
    box-shadow: var(--shadow-sm);
    transition: var(--transition);
}

.product-action-btn:hover {
    background: var(--accent);
    color: var(--white);
    transform: scale(1.1);
}

.product-info {
    padding: 20px;
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-direction: column;
    gap: 8px;
    flex: 1;
}

.product-category {
    font-size: 0.75rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    color: var(--accent);
    font-weight: 600;
}

.product-name {
    font-family: var(--font-heading);
    font-size: 1.1rem;
    font-weight: 600;
    color: var(--primary);
    line-height: 1.3;
}

.product-rating {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    gap: 8px;
}

.stars {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    gap: 2px;
    color: #f4c430;
    font-size: 0.8rem;
}

.product-rating span {
    font-size: 0.8rem;
    color: var(--gray);
}

.product-price {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    gap: 10px;
    margin-top: auto;
    padding-top: 8px;
}

.current-price {
    font-size: 1.15rem;
    font-weight: 700;
    color: var(--primary);
}

.original-price {
    font-size: 0.9rem;
    color: var(--gray);
    text-decoration: line-through;
}

.products-cta {
    text-align: center;
    margin-top: 48px;
}

/* ===================== PROMO BANNER ===================== */
.promo-banner {
    position: relative;
    min-height: 500px;
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
}

.promo-bg {
    position: absolute;
    inset: 0;
}

.promo-bg-img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.promo-overlay {
    position: absolute;
    inset: 0;
    background: linear-gradient(135deg, rgba(26, 26, 46, 0.9), rgba(22, 33, 62, 0.75));
}

.promo-content {
    position: relative;
    z-index: 2;
    text-align: center;
    color: var(--white);
    padding: 60px 24px;
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-direction: column;
    align-items: center;
}

.promo-tag {
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 3px;
    color: var(--accent);
    font-weight: 600;
    margin-bottom: 20px;
}

.promo-title {
    font-family: var(--font-heading);
    font-size: clamp(2rem, 5vw, 3.5rem);
    font-weight: 700;
    margin-bottom: 16px;
    line-height: 1.2;
}

.promo-highlight { color: var(--accent); }

.promo-text {
    font-size: 1.05rem;
    color: rgba(255, 255, 255, 0.75);
    max-width: 480px;
    margin-bottom: 36px;
}

/* Countdown */
.countdown {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    gap: 20px;
    margin-bottom: 36px;
}

.countdown-item {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-direction: column;
    align-items: center;
    background: rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 255, 255, 0.15);
    border-radius: var(--radius-md);
    padding: 16px 22px;
    min-width: 80px;
}

.countdown-num {
    font-family: var(--font-heading);
    font-size: 2rem;
    font-weight: 700;
    color: var(--accent);
    line-height: 1;
}

.countdown-label {
    font-size: 0.7rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    color: rgba(255, 255, 255, 0.6);
    margin-top: 6px;
}

/* ===================== FEATURES (FLEXBOX GRID) ===================== */
.features {
    padding: var(--section-padding);
    background: var(--white);
}

.features-grid {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-wrap: wrap;
    gap: var(--gap);
}

.feature-card {
    flex: 1 1 calc(33.333% - var(--gap));
    min-width: 280px;
    text-align: center;
    padding: 40px 30px;
    border-radius: var(--radius-md);
    background: var(--off-white);
    transition: var(--transition);
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-direction: column;
    align-items: center;
}

.feature-card:hover {
    transform: translateY(-6px);
    box-shadow: var(--shadow-md);
    background: var(--white);
}

.feature-icon {
    width: 72px;
    height: 72px;
    border-radius: var(--radius-full);
    background: var(--accent-light);
    /* ★ FLEXBOX centering ★ */
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 20px;
    font-size: 1.5rem;
    color: var(--accent);
    transition: var(--transition);
}

.feature-card:hover .feature-icon {
    background: var(--accent);
    color: var(--white);
    transform: scale(1.1);
}

.feature-card h3 {
    font-family: var(--font-heading);
    font-size: 1.2rem;
    font-weight: 600;
    margin-bottom: 10px;
    color: var(--primary);
}

.feature-card p {
    font-size: 0.9rem;
    color: var(--text-light);
    line-height: 1.7;
}

/* ===================== TESTIMONIALS ===================== */
.testimonials {
    padding: var(--section-padding);
    background: var(--off-white);
}

.testimonial-slider {
    max-width: 900px;
    margin: 0 auto;
    overflow: hidden;
}

.testimonial-track {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    transition: transform 0.5s cubic-bezier(0.4, 0, 0.2, 1);
}

.testimonial-card {
    min-width: 100%;
    padding: 48px 40px;
    text-align: center;
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-direction: column;
    align-items: center;
}

.testimonial-stars {
    /* ★ FLEXBOX ★ */
    display: flex;
    gap: 4px;
    color: #f4c430;
    font-size: 1.1rem;
    margin-bottom: 24px;
}

.testimonial-text {
    font-family: var(--font-heading);
    font-size: 1.3rem;
    font-weight: 400;
    color: var(--primary);
    line-height: 1.8;
    font-style: italic;
    max-width: 650px;
    margin-bottom: 32px;
}

.testimonial-author {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    gap: 14px;
}

.author-img {
    width: 52px;
    height: 52px;
    border-radius: var(--radius-full);
    object-fit: cover;
    border: 3px solid var(--accent);
}

.testimonial-author h4 {
    font-size: 1rem;
    font-weight: 600;
    color: var(--primary);
}

.testimonial-author span {
    font-size: 0.8rem;
    color: var(--accent);
    font-weight: 500;
}

.testimonial-nav {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 24px;
    margin-top: 20px;
}

.testimonial-btn {
    width: 44px;
    height: 44px;
    border-radius: var(--radius-full);
    border: 2px solid var(--light-gray);
    /* ★ FLEXBOX centering ★ */
    display: flex;
    align-items: center;
    justify-content: center;
    color: var(--text-light);
    font-size: 0.9rem;
}

.testimonial-btn:hover {
    border-color: var(--accent);
    color: var(--accent);
    background: var(--accent-light);
}

.testimonial-dots {
    /* ★ FLEXBOX ★ */
    display: flex;
    gap: 8px;
}

.dot {
    width: 10px;
    height: 10px;
    border-radius: var(--radius-full);
    background: var(--light-gray);
    cursor: pointer;
    transition: var(--transition);
}

.dot.active {
    background: var(--accent);
    width: 28px;
    border-radius: 10px;
}

/* ===================== NEWSLETTER (FLEXBOX) ===================== */
.newsletter {
    padding: var(--section-padding);
    background: var(--primary);
    color: var(--white);
}

.newsletter-flex {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 60px;
}

.newsletter-content {
    flex: 1;
}

.newsletter-content .section-tag {
    color: var(--accent);
}

.newsletter-title {
    font-family: var(--font-heading);
    font-size: clamp(1.8rem, 3vw, 2.5rem);
    font-weight: 700;
    margin: 12px 0 16px;
}

.newsletter-content p {
    color: rgba(255, 255, 255, 0.7);
    font-size: 1rem;
    max-width: 420px;
}

.newsletter-form {
    flex: 1;
    max-width: 480px;
}

.input-group {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    background: rgba(255, 255, 255, 0.1);
    border: 1px solid rgba(255, 255, 255, 0.15);
    border-radius: 50px;
    overflow: hidden;
    padding: 6px;
}

.newsletter-input {
    flex: 1;
    border: none;
    outline: none;
    background: transparent;
    padding: 12px 20px;
    font-size: 0.95rem;
    color: var(--white);
    font-family: inherit;
}

.newsletter-input::placeholder {
    color: rgba(255, 255, 255, 0.4);
}

.newsletter-disclaimer {
    font-size: 0.8rem;
    color: rgba(255, 255, 255, 0.4);
    margin-top: 14px;
    text-align: center;
}

.newsletter-disclaimer i {
    margin-right: 6px;
}

/* ===================== INSTAGRAM FEED (FLEXBOX) ===================== */
.instagram-feed {
    padding: 80px 0 0;
    background: var(--white);
}

.instagram-feed .section-header {
    margin-bottom: 40px;
}

.insta-grid {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
}

.insta-item {
    flex: 1;
    position: relative;
    overflow: hidden;
    aspect-ratio: 1;
}

.insta-item img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: var(--transition-slow);
}

.insta-item:hover img {
    transform: scale(1.1);
}

.insta-overlay {
    position: absolute;
    inset: 0;
    background: rgba(201, 169, 110, 0.8);
    /* ★ FLEXBOX centering ★ */
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: var(--transition);
}

.insta-overlay i {
    font-size: 2rem;
    color: var(--white);
    transform: scale(0.5);
    transition: var(--transition);
}

.insta-item:hover .insta-overlay {
    opacity: 1;
}

.insta-item:hover .insta-overlay i {
    transform: scale(1);
}

/* ===================== FOOTER (FLEXBOX) ===================== */
.footer {
    background: var(--primary);
    color: rgba(255, 255, 255, 0.75);
    padding: 80px 0 0;
}

.footer-grid {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-wrap: wrap;
    gap: 48px;
    padding-bottom: 60px;
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.footer-brand {
    flex: 1 1 300px;
    max-width: 340px;
}

.footer-col {
    flex: 1 1 180px;
}

.footer-logo {
    font-family: var(--font-heading);
    font-size: 1.5rem;
    font-weight: 700;
    color: var(--white);
    letter-spacing: 3px;
    /* ★ FLEXBOX ★ */
    display: flex;
    align-items: center;
    gap: 4px;
    margin-bottom: 16px;
}

.footer-brand p {
    font-size: 0.9rem;
    line-height: 1.8;
    margin-bottom: 24px;
}

.footer-social {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    gap: 10px;
}

.social-link {
    width: 40px;
    height: 40px;
    border-radius: var(--radius-full);
    border: 1px solid rgba(255, 255, 255, 0.15);
    /* ★ FLEXBOX centering ★ */
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.9rem;
    color: rgba(255, 255, 255, 0.6);
    transition: var(--transition);
}

.social-link:hover {
    background: var(--accent);
    border-color: var(--accent);
    color: var(--white);
    transform: translateY(-3px);
}

.footer-col h4 {
    font-family: var(--font-heading);
    font-size: 1.1rem;
    font-weight: 600;
    color: var(--white);
    margin-bottom: 24px;
}

.footer-col ul {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    flex-direction: column;
    gap: 12px;
}

.footer-col ul li a {
    font-size: 0.9rem;
    color: rgba(255, 255, 255, 0.6);
    transition: var(--transition);
    /* ★ FLEXBOX ★ */
    display: flex;
    align-items: center;
    gap: 10px;
}

.footer-col ul li a:hover {
    color: var(--accent);
    transform: translateX(4px);
}

.contact-list li {
    font-size: 0.9rem;
    /* ★ FLEXBOX ★ */
    display: flex;
    align-items: flex-start;
    gap: 10px;
}

.contact-list i {
    color: var(--accent);
    margin-top: 4px;
    min-width: 16px;
}

.footer-bottom {
    padding: 24px 0;
}

.footer-bottom-flex {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 20px;
}

.footer-bottom p {
    font-size: 0.85rem;
    color: rgba(255, 255, 255, 0.4);
}

.footer-links {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    gap: 24px;
}

.footer-links a {
    font-size: 0.85rem;
    color: rgba(255, 255, 255, 0.4);
}

.footer-links a:hover {
    color: var(--accent);
}

.payment-methods {
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    gap: 16px;
    font-size: 1.5rem;
    color: rgba(255, 255, 255, 0.3);
}

/* ===================== BACK TO TOP ===================== */
.back-to-top {
    position: fixed;
    bottom: 30px;
    right: 30px;
    width: 48px;
    height: 48px;
    background: var(--accent);
    color: var(--white);
    border-radius: var(--radius-full);
    /* ★ FLEXBOX centering ★ */
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1rem;
    box-shadow: var(--shadow-md);
    opacity: 0;
    visibility: hidden;
    transform: translateY(20px);
    transition: var(--transition);
    z-index: 999;
}

.back-to-top.visible {
    opacity: 1;
    visibility: visible;
    transform: translateY(0);
}

.back-to-top:hover {
    background: var(--accent-hover);
    transform: translateY(-4px);
}

/* ===================== TOAST NOTIFICATION ===================== */
.toast {
    position: fixed;
    bottom: 30px;
    left: 50%;
    transform: translateX(-50%) translateY(100px);
    background: var(--primary);
    color: var(--white);
    padding: 16px 28px;
    border-radius: 50px;
    /* ★ FLEXBOX LAYOUT ★ */
    display: flex;
    align-items: center;
    gap: 10px;
    font-size: 0.9rem;
    font-weight: 500;
    box-shadow: var(--shadow-xl);
    z-index: 2000;
    opacity: 0;
    transition: var(--transition);
}

.toast.show {
    transform: translateX(-50%) translateY(0);
    opacity: 1;
}

.toast i {
    color: var(--success);
    font-size: 1.1rem;
}

/* ===================== ANIMATIONS ===================== */
@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.reveal {
    opacity: 0;
    transform: translateY(40px);
    transition: opacity 0.8s ease, transform 0.8s ease;
}

.reveal.active {
    opacity: 1;
    transform: translateY(0);
}

/* ===================== RESPONSIVE DESIGN ===================== */

/* Tablet Landscape */
@media (max-width: 1024px) {
    .nav-links { gap: 24px; }

    .product-card {
        flex: 1 1 calc(33.333% - var(--gap));
    }

    .category-card.category-large,
    .category-card.category-wide {
        flex: 1 1 100%;
    }

    .category-card {
        flex: 1 1 calc(50% - var(--gap));
    }

    .newsletter-flex {
        flex-direction: column;
        text-align: center;
    }

    .newsletter-content p { margin: 0 auto; }

    .newsletter-form { max-width: 100%; width: 100%; }
}

/* Tablet Portrait */
@media (max-width: 768px) {
    :root {
        --section-padding: 70px 0;
        --gap: 16px;
    }

    /* Mobile Navigation */
    .hamburger {
        display: flex;
    }

    .nav-links {
        position: fixed;
        top: 0;
        right: -100%;
        width: 300px;
        height: 100vh;
        background: var(--primary);
        /* ★ FLEXBOX LAYOUT (vertical) ★ */
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 32px;
        z-index: 999;
        transition: var(--transition);
    }

    .nav-links.active { right: 0; }

    .nav-link {
        color: rgba(255, 255, 255, 0.85);
        font-size: 1.1rem;
    }

    .hero-stats {
        gap: 24px;
    }

    .stat-number { font-size: 1.6rem; }

    .product-card {
        flex: 1 1 calc(50% - var(--gap));
    }

    .feature-card {
        flex: 1 1 calc(50% - var(--gap));
    }

    .footer-grid { gap: 32px; }

    .footer-brand { max-width: 100%; }

    .footer-bottom-flex {
        flex-direction: column;
        text-align: center;
    }

    .insta-grid {
        flex-wrap: wrap;
    }

    .insta-item {
        flex: 1 1 calc(33.333%);
    }

    .countdown-item { padding: 12px 16px; min-width: 65px; }
    .countdown-num { font-size: 1.5rem; }

    .testimonial-card { padding: 30px 20px; }
    .testimonial-text { font-size: 1.1rem; }
}

/* Mobile */
@media (max-width: 480px) {
    :root {
        --section-padding: 56px 0;
    }

    .announcement-bar { font-size: 0.75rem; padding: 8px 12px; }

    .logo { font-size: 1.4rem; }

    .hero-title { font-size: 2rem; }
    .hero-subtitle { font-size: 0.95rem; }

    .hero-cta {
        flex-direction: column;
        width: 100%;
        padding: 0 20px;
    }

    .hero-cta .btn { width: 100%; justify-content: center; }

    .hero-stats {
        flex-direction: column;
        gap: 16px;
    }

    .product-card {
        flex: 1 1 100%;
    }

    .feature-card {
        flex: 1 1 100%;
    }

    .category-card,
    .category-card.category-large,
    .category-card.category-wide {
        flex: 1 1 100%;
        min-height: 220px;
    }

    .input-group {
        flex-direction: column;
        border-radius: var(--radius-md);
        gap: 8px;
    }

    .input-group .btn {
        border-radius: 50px;
        justify-content: center;
    }

    .insta-item { flex: 1 1 50%; }

    .countdown { gap: 10px; }
    .countdown-item { padding: 10px 12px; min-width: 55px; }
    .countdown-num { font-size: 1.2rem; }

    .section-title { font-size: 1.75rem; }

    .footer-col { flex: 1 1 100%; }

    .footer-links {
        flex-direction: column;
        gap: 10px;
    }

    .payment-methods { justify-content: center; }
}
```

## OUTPUT
![alt text](<Screenshot (75).png>)
![alt text](<Screenshot (76).png>)
![alt text](<Screenshot (78).png>)
![alt text](<Screenshot (77).png>)
![alt text](<Screenshot (79).png>)
![alt text](<Screenshot (80).png>)
## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
