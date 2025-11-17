<script setup lang="ts">

</script>

<template>
  <!DOCTYPE html>
  <html lang="ru">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MotoStore - Магазин мотоаксессуаров</title>

  </head>
  <div class="main-container">
  <!-- Шапка сайта -->
  <header>
    <div class="container header-content">
      <div class="logo">Moto<span>Store</span></div>
      <nav>
        <ul>
          <li><a href="#">Главная</a></li>
          <li><a href="#">Экипировка</a></li>
          <li><a href="#">Запчасти</a></li>
          <li><a href="#">Аксессуары</a></li>
          <li><a href="#">О нас</a></li>
          <li class="cart-icon">
            Корзина
            <span class="cart-count">0</span>
          </li>
        </ul>
      </nav>
    </div>
  </header>

  <!-- Главный баннер -->
  <section class="hero">
    <div class="container">
      <h1>Мотоаксессуары для настоящих байкеров</h1>
      <p>Качественная экипировка, запчасти и аксессуары для вашего железного коня</p>
      <a href="#" class="btn">Смотреть каталог</a>
    </div>
  </section>

  <!-- Секция товаров -->
  <section class="products">
    <div class="container">
      <h2 class="section-title">Популярные товары</h2>
      <div class="product-grid">
        <!-- Товар 1 -->
        <div class="product-card">
          <div class="product-image">
            <img src="https://images.unsplash.com/photo-1628149330013-90e8a987969b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Мотошлем">
          </div>
          <div class="product-info">
            <h3 class="product-title">Шлем AGV Sport Modular</h3>
            <p class="product-price">24 999 ₽</p>
            <p class="product-description">Спортивный модульный шлем с системой вентиляции и защитой от запотевания</p>
            <button class="add-to-cart">В корзину</button>
          </div>
        </div>

        <!-- Товар 2 -->
        <div class="product-card">
          <div class="product-image">
            <img src="https://images.unsplash.com/photo-1628149330106-6433a66d4769?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Куртка кожаная">
          </div>
          <div class="product-info">
            <h3 class="product-title">Кожаная куртка MotoStyle</h3>
            <p class="product-price">18 500 ₽</p>
            <p class="product-description">Классическая кожаная куртка с защитой на плечах и локтях</p>
            <button class="add-to-cart">В корзину</button>
          </div>
        </div>

        <!-- Товар 3 -->
        <div class="product-card">
          <div class="product-image">
            <img src="https://images.unsplash.com/photo-1571068316343-3a1c16c407e3?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Перчатки">
          </div>
          <div class="product-info">
            <h3 class="product-title">Перчатки Alpinestars GP Pro</h3>
            <p class="product-price">7 800 ₽</p>
            <p class="product-description">Спортивные перчатки с защитой костяшек и карбоновыми вставками</p>
            <button class="add-to-cart">В корзину</button>
          </div>
        </div>

        <!-- Товар 4 -->
        <div class="product-card">
          <div class="product-image">
            <img src="https://images.unsplash.com/photo-1558618047-3c8c76ca7d13?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Выхлопная система">
          </div>
          <div class="product-info">
            <h3 class="product-title">Выхлопная система Yoshimura</h3>
            <p class="product-price">42 500 ₽</p>
            <p class="product-description">Титановая выхлопная система для увеличения мощности и улучшения звука</p>
            <button class="add-to-cart">В корзину</button>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Подвал -->
  <footer>
    <div class="container">
      <div class="footer-content">
        <div class="footer-section">
          <h3>О компании</h3>
          <p>MotoStore - магазин для настоящих байкеров. Мы предлагаем качественную экипировку, запчасти и аксессуары для мотоциклов.</p>
          <div class="social-links">
            <a href="#">VK</a>
            <a href="#">TG</a>
            <a href="#">YT</a>
            <a href="#">IG</a>
          </div>
        </div>
        <div class="footer-section">
          <h3>Категории</h3>
          <ul>
            <li><a href="#">Шлемы</a></li>
            <li><a href="#">Куртки</a></li>
            <li><a href="#">Перчатки</a></li>
            <li><a href="#">Выхлопные системы</a></li>
            <li><a href="#">Запчасти</a></li>
          </ul>
        </div>
        <div class="footer-section">
          <h3>Контакты</h3>
          <ul>
            <li>Телефон: +7 (999) 777-77-77</li>
            <li>Email: info@motostore.ru</li>
            <li>Адрес: г. Москва, ш. Энтузиастов, д. 12</li>
            <li>Режим работы: 10:00 - 22:00</li>
          </ul>
        </div>
      </div>
      <div class="copyright">
        <p>&copy; 2023 MotoStore. Все права защищены.</p>
      </div>
    </div>
  </footer>

<!--  <script>-->
<!--    // Функционал для корзины-->
<!--    document.addEventListener('DOMContentLoaded', function() {-->
<!--      const addToCartButtons = document.querySelectorAll('.add-to-cart');-->
<!--      const cartCount = document.querySelector('.cart-count');-->
<!--      let count = 0;-->

<!--      addToCartButtons.forEach(button => {-->
<!--        button.addEventListener('click', function() {-->
<!--          count++;-->
<!--          cartCount.textContent = count;-->

<!--          // Анимация добавления в корзину-->
<!--          const originalText = this.textContent;-->
<!--          this.textContent = 'Добавлено!';-->
<!--          this.style.backgroundColor = '#32CD32';-->

<!--          setTimeout(() => {-->
<!--            this.textContent = originalText;-->
<!--            this.style.backgroundColor = '#ff4500';-->
<!--          }, 1500);-->
<!--        });-->
<!--      });-->
<!--    });-->
<!--  </script>-->
  </div>
  </html>
</template>

<style scoped>
  /* Общие стили */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

  .main-container {
  background-color: #0a0a0a;
  color: #f0f0f0;
  line-height: 1.6;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

/* Шапка сайта */
header {
  background-color: #000;
  color: #f0f0f0;
  padding: 1rem 0;
  box-shadow: 0 2px 10px rgba(255, 69, 0, 0.3);
  border-bottom: 2px solid #ff4500;
}

.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.8rem;
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 2px;
}

.logo span {
  color: #ff4500;
}

nav ul {
  display: flex;
  list-style: none;
}

nav ul li {
  margin-left: 1.5rem;
}

nav ul li a {
  color: #f0f0f0;
  text-decoration: none;
  transition: color 0.3s;
  font-weight: 500;
  text-transform: uppercase;
  font-size: 0.9rem;
  letter-spacing: 1px;
}

nav ul li a:hover {
  color: #ff4500;
}

.cart-icon {
  position: relative;
  cursor: pointer;
  display: flex;
  align-items: center;
}

.cart-count {
  position: absolute;
  top: -8px;
  right: -8px;
  background-color: #ff4500;
  color: #000;
  border-radius: 50%;
  width: 18px;
  height: 18px;
  font-size: 0.7rem;
  display: flex;
  justify-content: center;
  align-items: center;
  font-weight: bold;
}

/* Главный баннер */
.hero {
  background: #0a0a0a;
  background-size: cover;
  background-position: center;
  color: #f0f0f0;
  padding: 5rem 0;
  text-align: center;
  margin-bottom: 2rem;
  border-bottom: 2px solid #ff4500;
}

.hero h1 {
  font-size: 3rem;
  margin-bottom: 1rem;
  text-transform: uppercase;
  letter-spacing: 2px;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.8);
}

.hero p {
  font-size: 1.2rem;
  max-width: 600px;
  margin: 0 auto 1.5rem;
}

.btn {
  display: inline-block;
  background-color: #ff4500;
  color: #000;
  padding: 0.8rem 1.5rem;
  border: none;
  border-radius: 4px;
  text-decoration: none;
  font-weight: bold;
  cursor: pointer;
  transition: all 0.3s;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-size: 0.9rem;
}

.btn:hover {
  background-color: #ff5500;
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(255, 69, 0, 0.4);
}

/* Секция товаров */
.products {
  background: #0a0a0a;
  padding: 3rem 0;
}

.section-title {
  text-align: center;
  margin-bottom: 2rem;
  font-size: 2rem;
  color: #f0f0f0;
  text-transform: uppercase;
  letter-spacing: 2px;
  position: relative;
}

.section-title:after {
  content: '';
  display: block;
  width: 100px;
  height: 3px;
  background-color: #ff4500;
  margin: 10px auto;
}

.product-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 2rem;
}

.product-card {
  background-color: #1a1a1a;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 3px 15px rgba(0,0,0,0.5);
  transition: transform 0.3s, box-shadow 0.3s;
  border: 1px solid #333;
}

.product-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 20px rgba(255, 69, 0, 0.3);
  border-color: #ff4500;
}

.product-image {
  height: 220px;
  background-color: #000;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  border-bottom: 2px solid #ff4500;
}

.product-image img {
  max-width: 100%;
  max-height: 100%;
  object-fit: cover;
  transition: transform 0.5s;
}

.product-card:hover .product-image img {
  transform: scale(1.05);
}

.product-info {
  padding: 1.5rem;
}

.product-title {
  font-size: 1.2rem;
  margin-bottom: 0.5rem;
  color: #f0f0f0;
}

.product-price {
  font-size: 1.4rem;
  font-weight: bold;
  color: #ff4500;
  margin-bottom: 1rem;
}

.product-description {
  color: #aaa;
  margin-bottom: 1rem;
  font-size: 0.9rem;
  line-height: 1.5;
}

.add-to-cart {
  width: 100%;
  padding: 0.8rem;
  background-color: #ff4500;
  color: #000;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-weight: bold;
  transition: background-color 0.3s;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.add-to-cart:hover {
  background-color: #ff5500;
}

/* Подвал */
footer {
  background-color: #000;
  color: #f0f0f0;
  padding: 3rem 0 1.5rem;
  margin-top: 3rem;
  border-top: 2px solid #ff4500;
}

.footer-content {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  margin-bottom: 2rem;
}

.footer-section {
  flex: 1;
  min-width: 250px;
  margin-bottom: 1.5rem;
}

.footer-section h3 {
  margin-bottom: 1rem;
  font-size: 1.2rem;
  color: #ff4500;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.footer-section ul {
  list-style: none;
}

.footer-section ul li {
  margin-bottom: 0.5rem;
}

.footer-section ul li a {
  color: #aaa;
  text-decoration: none;
  transition: color 0.3s;
}

.footer-section ul li a:hover {
  color: #ff4500;
}

.social-links {
  display: flex;
  gap: 1rem;
  margin-top: 1rem;
}

.social-links a {
  display: inline-block;
  width: 36px;
  height: 36px;
  background-color: #333;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: background-color 0.3s;
}

.social-links a:hover {
  background-color: #ff4500;
}

.copyright {
  text-align: center;
  margin-top: 2rem;
  padding-top: 1.5rem;
  border-top: 1px solid #333;
  color: #777;
  font-size: 0.9rem;
}

/* Адаптивность */
@media (max-width: 768px) {
  .header-content {
    flex-direction: column;
    text-align: center;
  }

  nav ul {
    margin-top: 1rem;
    justify-content: center;
  }

  .hero h1 {
    font-size: 2.2rem;
  }

  .hero p {
    font-size: 1rem;
  }

  .footer-content {
    flex-direction: column;
  }
}

@media (max-width: 480px) {
  .product-grid {
    grid-template-columns: 1fr;
  }

  nav ul {
    flex-wrap: wrap;
  }

  nav ul li {
    margin: 0.5rem;
  }
}
</style>
