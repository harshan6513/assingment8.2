
/* Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Page styling */
body {
    font-family: Arial, sans-serif;
    background-color: #f4f7fb;
    color: #222;
}

/* Header */
.header {
    text-align: center;
    padding: 40px 20px;
    background: linear-gradient(135deg, #173b65, #3979a8);
    color: white;
}

.header h1 {
    font-size: 36px;
    margin-bottom: 10px;
}

.header p {
    font-size: 16px;
    color: #e5edf5;
}

/* Gallery container */
.gallery-container {
    max-width: 1200px;
    margin: 35px auto;
    padding: 0 20px;
}

/* Responsive Grid */
.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 24px;
}

/* Individual gallery item */
.gallery-item {
    background-color: white;
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.10);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.gallery-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
}

/* Images */
.gallery-item img {
    display: block;
    width: 100%;
    height: 220px;
    object-fit: cover;
}

.gallery-item h3 {
    text-align: center;
    padding: 16px 10px;
    font-size: 18px;
}

/* Footer */
footer {
    text-align: center;
    padding: 22px 12px;
    background-color: #173b65;
    color: white;
    margin-top: 40px;
}

/* Mobile adjustments */
@media (max-width: 480px) {
    .header {
        padding: 30px 15px;
    }

    .header h1 {
        font-size: 28px;
    }

    .gallery-container {
        padding: 0 14px;
        margin: 24px auto;
    }

    .gallery {
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 16px;
    }

    .gallery-item img {
        height: 200px;
    }
}
