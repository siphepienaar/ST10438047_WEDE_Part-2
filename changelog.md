index.html
What changes did you make on this html
- [2025-09-23] Fixed navigation menu (all links working).
- [2025-09-23] Added comments in HTML code for clarity.
- [2025-09-23] Improved responsiveness with media queries.
- [2025-09-23] Updated references (added in-text referencing).

CSS
/* ==============================
   RESET & BASE STYLES
   ============================== */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', Arial, sans-serif;
  font-size: 16px;
  line-height: 1.6;
  background-color: #fafafa;
  color: #222;
}

/* Links */
a {
  text-decoration: none;
  color: inherit;
}

img {
  max-width: 100%;
  height: auto;
  border-radius: 8px;
}

/* ==============================
   HEADER & NAVIGATION
   ============================== */
header {
  background: #000;
  color: #fff;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 30px;
  position: sticky;
  top: 0;
  z-index: 1000;
}

header img {
  max-height: 60px;
}

nav a {
  margin-left: 20px;
  color: #fff;
  font-weight: bold;
  transition: color 0.3s ease;
}

nav a:hover {
  color: #9b5de5; /* aespa purple */
}

/* ==============================
   MAIN CONTENT
   ============================== */
main {
  padding: 30px;
  text-align: center;
}

main h1 {
  font-size: 2.5rem;
  margin-bottom: 15px;
  color: #111;
}

main p {
  font-size: 1.1rem;
  margin-bottom: 20px;
  color: #444;
}

button {
  background: #9b5de5;
  border: none;
  padding: 10px 20px;
  color: white;
  font-size: 1rem;
  font-weight: bold;
  border-radius: 6px;
  cursor: pointer;
  transition: background 0.3s ease;
}

button:hover {
  background: #7a3cc2;
}

/* ==============================
   FOOTER
   ============================== */
footer {
  background: #111;
  color: #fff;
  text-align: center;
  padding: 15px;
  margin-top: 40px;
  font-size: 0.9rem;
}

/* ==============================
   PRODUCTS GRID
   ============================== */
.products-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 20px;
  margin-top: 20px;
}

.product-card {
  background: #fff;
  padding: 15px;
  border-radius: 10px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
}

.product-card:hover {
  transform: translateY(-5px);
}

.product-card img {
  margin-bottom: 10px;
}

/* ==============================
   RESPONSIVE DESIGN
   ============================== */

/* Tablet */
@media (max-width: 768px) {
  header {
    flex-direction: column;
    text-align: center;
  }
  
  nav {
    margin-top: 10px;
  }
  
  nav a {
    display: inline-block;
    margin: 8px 10px;
  }
  
  main h1 {
    font-size: 2rem;
  }
}

/* Mobile */
@media (max-width: 480px) {
  body {
    font-size: 14px;
  }
  
  header {
    padding: 10px;
  }
  
  nav a {
    display: block;
    margin: 5px 0;
  }
  
  main {
    padding: 15px;
  }
  
  main h1 {
    font-size: 1.6rem;
  }
  
  footer {
    font-size: 0.8rem;
  }
}


Bug or errors
