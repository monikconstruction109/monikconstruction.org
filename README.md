 {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --primary-color: #1e3a5f;
    --secondary-color: #ff6b35;
    --text-color: #333;
    --light-bg: #f8f9fa;
    --white: #ffffff;
    --border-color: #e0e0e0;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: var(--text-color);
}

/* Container */
.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Header & Navigation */
header {
    background: var(--primary-color);
    color: var(--white);
    padding: 1rem 0;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

header .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 1.5rem;
    font-weight: bold;
}

nav ul {
    list-style: none;
    display: flex;
    gap: 2rem;
}

nav a {
    color: var(--white);
    text-decoration: none;
    font-weight: 500;
    transition: color 0.3s ease;
}

nav a:hover {
    color: var(--secondary-color);
}

/* Hero Section */
.hero {
    background: linear-gradient(135deg, var(--primary-color) 0%, #2d5a8c 100%);
    color: var(--white);
    padding: 100px 20px;
    text-align: center;
}

.hero-content h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
    line-height: 1.2;
}

.hero-content p {
    font-size: 1.3rem;
    margin-bottom: 2rem;
    opacity: 0.95;
}

/* Button */
.btn {
    display: inline-block;
    background: var(--secondary-color);
    color: var(--white);
    padding: 12px 30px;
    border-radius: 5px;
    text-decoration: none;
    font-weight: bold;
    transition: all 0.3s ease;
    border: none;
    cursor: pointer;
    font-size: 1rem;
}

.btn:hover {
    background: #e55a2b;
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(255, 107, 53, 0.4);
}

/* Sections */
.section {
    padding: 60px 20px;
}

.section h2 {
    font-size: 2.5rem;
    margin-bottom: 2rem;
    color: var(--primary-color);
    text-align: center;
}

.section p {
    font-size: 1.1rem;
    line-height: 1.8;
    color: #555;
}

/* Light Background */
.light {
    background: var(--light-bg);
}

/* Services Cards */
.cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
}

.card {
    background: var(--white);
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    transition: all 0.3s ease;
    border-top: 4px solid var(--secondary-color);
}

.card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
}

.card h3 {
    color: var(--primary-color);
    margin-bottom: 1rem;
    font-size: 1.3rem;
}

.card p {
    color: #666;
}

/* Contact Section */
.contact-info {
    background: var(--light-bg);
    padding: 2rem;
    border-radius: 8px;
    margin-bottom: 2rem;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1.5rem;
}

.contact-info p {
    font-size: 1rem;
}

.contact-info strong {
    color: var(--primary-color);
}

/* Contact Form */
form {
    background: var(--light-bg);
    padding: 2rem;
    border-radius: 8px;
    max-width: 600px;
    margin: 0 auto;
}

form input,
form textarea {
    width: 100%;
    padding: 12px;
    margin-bottom: 1rem;
    border: 1px solid var(--border-color);
    border-radius: 5px;
    font-family: inherit;
    font-size: 1rem;
    transition: border-color 0.3s ease;
}

form input:focus,
form textarea:focus {
    outline: none;
    border-color: var(--secondary-color);
    box-shadow: 0 0 5px rgba(255, 107, 53, 0.3);
}

form button {
    width: 100%;
    padding: 12px;
    background: var(--secondary-color);
    color: var(--white);
    border: none;
    border-radius: 5px;
    font-size: 1rem;
    font-weight: bold;
    cursor: pointer;
    transition: all 0.3s ease;
}

form button:hover {
    background: #e55a2b;
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(255, 107, 53, 0.4);
}

/* Footer */
footer {
    background: var(--primary-color);
    color: var(--white);
    text-align: center;
    padding: 2rem;
    margin-top: 3rem;
}

/* Responsive Design */
@media (max-width: 768px) {
    header .container {
        flex-direction: column;
        gap: 1rem;
    }

    nav ul {
        gap: 1rem;
        flex-wrap: wrap;
        justify-content: center;
    }

    .hero-content h1 {
        font-size: 2rem;
    }

    .hero-content p {
        font-size: 1rem;
    }

    .section h2 {
        font-size: 2rem;
    }

    .cards {
        grid-template-columns: 1fr;
    }

    .contact-info {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 480px) {
    .hero-content h1 {
        font-size: 1.5rem;
    }

    .section h2 {
        font-size: 1.5rem;
    }

    nav ul {
        gap: 0.5rem;
    }

    nav a {
        font-size: 0.9rem;
    }
}
