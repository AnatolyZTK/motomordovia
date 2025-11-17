<script setup lang="ts">

</script>

<template>
  <div class="product-container">
  <!-- Шапка сайта -->
  <header>
    <div class="container header-content">
      <div class="logo">Moto<span>Store</span></div>
      <nav>
        <ul>
          <li><a href="#">Главная</a></li>
          <li><a href="#">Каталог</a></li>
          <li><a href="#">Экипировка</a></li>
          <li><a href="#">Запчасти</a></li>
          <li><a href="#">Аксессуары</a></li>
          <li class="cart-icon">
            Корзина
            <span class="cart-count">2</span>
          </li>
        </ul>
      </nav>
    </div>
  </header>

  <!-- Хлебные крошки -->
  <div class="container breadcrumbs">
    <a href="#">Главная</a> <span>></span> <a href="#">Каталог</a> <span>></span> <a href="#">Шлемы</a> <span>></span> <span>Шлем AGV Sport Modular</span>
  </div>

  <!-- Карточка товара -->
  <div class="container product-detail">
    <div class="product-gallery">
      <div class="main-image">
        <img src="https://images.unsplash.com/photo-1628149330013-90e8a987969b?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Шлем AGV Sport Modular" id="main-image">
      </div>
      <div class="image-thumbnails">
        <div class="thumbnail active" data-image="https://images.unsplash.com/photo-1628149330013-90e8a987969b?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80">
          <img src="https://images.unsplash.com/photo-1628149330013-90e8a987969b?ixlib=rb-1.2.1&auto=format&fit=crop&w=150&q=80" alt="Шлем AGV вид 1">
        </div>
        <div class="thumbnail" data-image="https://images.unsplash.com/photo-1558618047-3c8c76ca7d13?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80">
          <img src="https://images.unsplash.com/photo-1558618047-3c8c76ca7d13?ixlib=rb-1.2.1&auto=format&fit=crop&w=150&q=80" alt="Шлем AGV вид 2">
        </div>
        <div class="thumbnail" data-image="https://images.unsplash.com/photo-1571068316343-3a1c16c407e3?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80">
          <img src="https://images.unsplash.com/photo-1571068316343-3a1c16c407e3?ixlib=rb-1.2.1&auto=format&fit=crop&w=150&q=80" alt="Шлем AGV вид 3">
        </div>
        <div class="thumbnail" data-image="https://images.unsplash.com/photo-1609630875171-b1321377ee65?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80">
          <img src="https://images.unsplash.com/photo-1609630875171-b1321377ee65?ixlib=rb-1.2.1&auto=format&fit=crop&w=150&q=80" alt="Шлем AGV вид 4">
        </div>
      </div>
    </div>

    <div class="product-info">
      <div class="product-category">Шлемы</div>
      <h1 class="product-title">Шлем AGV Sport Modular</h1>

      <div class="product-rating">
        <div class="stars">★★★★★</div>
        <div class="rating-count">4.8 (124 отзыва)</div>
      </div>

      <div class="product-price">24 999 ₽</div>

      <div class="product-description">
        Спортивный модульный шлем AGV Sport Modular сочетает в себе удобство открывания и безопасность интегральной конструкции. Оснащен продвинутой системой вентиляции, защитой от запотевания и современной системой крепления визора.
      </div>

      <div class="product-features">
        <h3 class="features-title">Основные особенности:</h3>
        <ul class="features-list">
          <li>Модульная конструкция с системой быстрого открывания</li>
          <li>Усовершенствованная система вентиляции с 5 воздухозаборниками</li>
          <li>Защита от запотевания с Pinlock® 100% Max Vision</li>
          <li>Внутренняя часть из гипоаллергенных материалов</li>
          <li>Сертификация ECE 22.06</li>
        </ul>
      </div>

      <div class="product-options">
        <h3 class="option-title">Размер:</h3>
        <div class="size-options">
          <div class="size-option">S</div>
          <div class="size-option active">M</div>
          <div class="size-option">L</div>
          <div class="size-option">XL</div>
        </div>

        <h3 class="option-title">Цвет:</h3>
        <div class="color-options">
          <div class="color-option color-black active"></div>
          <div class="color-option color-red"></div>
          <div class="color-option color-white"></div>
          <div class="color-option color-blue"></div>
        </div>
      </div>

      <div class="product-actions">
        <div class="quantity-selector">
          <button class="quantity-btn minus">-</button>
          <div class="quantity-value">1</div>
          <button class="quantity-btn plus">+</button>
        </div>
        <button class="add-to-cart">Добавить в корзину</button>
        <button class="buy-now">Купить сейчас</button>
      </div>

      <div class="product-meta">
        <div class="meta-item">
          <span>✓</span> В наличии
        </div>
        <div class="meta-item">
          <span>✓</span> Бесплатная доставка
        </div>
        <div class="meta-item">
          <span>✓</span> Гарантия 2 года
        </div>
      </div>
    </div>
  </div>

  <!-- Табы с дополнительной информацией -->
  <div class="container product-tabs">
    <div class="tabs-header">
      <button class="tab active" data-tab="description">Описание</button>
      <button class="tab" data-tab="specs">Характеристики</button>
      <button class="tab" data-tab="reviews">Отзывы (124)</button>
      <button class="tab" data-tab="delivery">Доставка</button>
    </div>

    <div class="tab-content active" id="description">
      <p>Шлем AGV Sport Modular - это идеальное сочетание комфорта, безопасности и стиля для современных мотоциклистов. Модульная конструкция позволяет легко преобразовывать шлем из интегрального в открытый, что особенно удобно в городских условиях.</p>
      <p>Внутренняя часть шлема выполнена из гипоаллергенных материалов, которые можно снимать и стирать. Система вентиляции включает 5 воздухозаборников и 2 вытяжных дефлектора, обеспечивая оптимальную циркуляцию воздуха в любых погодных условиях.</p>
      <p>Визор шлема оснащен системой быстрой замены и защитой от запотевания с использованием технологии Pinlock® 100% Max Vision, что гарантирует четкий обзор даже при резких перепадах температуры.</p>
    </div>

    <div class="tab-content" id="specs">
      <table class="specs-table">
        <tr>
          <td>Тип шлема</td>
          <td>Модульный</td>
        </tr>
        <tr>
          <td>Стандарт безопасности</td>
          <td>ECE 22.06</td>
        </tr>
        <tr>
          <td>Вес</td>
          <td>1550 г (±50 г)</td>
        </tr>
        <tr>
          <td>Количество вентиляционных отверстий</td>
          <td>5 воздухозаборников, 2 вытяжных дефлектора</td>
        </tr>
        <tr>
          <td>Материал корпуса</td>
          <td>Углеволокно</td>
        </tr>
        <tr>
          <td>Система визора</td>
          <td>Быстрая замена, Pinlock® 100% Max Vision</td>
        </tr>
        <tr>
          <td>Совместимость</td>
          <td>Система связи AGV (опционально)</td>
        </tr>
      </table>
    </div>

    <div class="tab-content" id="reviews">
      <div class="reviews-list">
        <div class="review">
          <div class="review-header">
            <div class="review-author">Александр Петров</div>
            <div class="review-date">15.03.2023</div>
          </div>
          <div class="review-rating">★★★★★</div>
          <p>Отличный шлем! Использую уже полгода, очень доволен. Качество сборки на высоте, удобно сидит, отличная вентиляция. Рекомендую!</p>
        </div>
        <div class="review">
          <div class="review-header">
            <div class="review-author">Дмитрий Иванов</div>
            <div class="review-date">02.02.2023</div>
          </div>
          <div class="review-rating">★★★★☆</div>
          <p>Хороший шлем за свои деньги. Удобный, легкий, отличный обзор. Единственный минус - немного шумный на высоких скоростях.</p>
        </div>
      </div>
    </div>

    <div class="tab-content" id="delivery">
      <p>Мы осуществляем доставку по всей России. Сроки доставки зависят от вашего региона:</p>
      <ul class="features-list">
        <li>Москва и область: 1-2 дня</li>
        <li>Другие регионы: 3-7 дней</li>
        <li>Отдаленные регионы: 7-14 дней</li>
      </ul>
      <p>При заказе от 5000 рублей доставка бесплатная. Также доступен самовывоз из наших магазинов в Москве и Санкт-Петербурге.</p>
    </div>
  </div>

  <!-- Похожие товары -->
  <div class="container related-products">
    <h2 class="section-title">Похожие товары</h2>
    <div class="products-grid">
      <!-- Товар 1 -->
      <div class="product-card">
        <div class="product-image">
          <img src="https://images.unsplash.com/photo-1558618667-3404e57f3b33?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Шлем Shark">
        </div>
        <div class="product-card-info">
          <h3 class="product-card-title">Шлем Shark Spartan</h3>
          <p class="product-card-price">21 500 ₽</p>
          <div class="product-card-actions">
            <button class="product-card-add-to-cart">В корзину</button>
          </div>
        </div>
      </div>

      <!-- Товар 2 -->
      <div class="product-card">
        <div class="product-image">
          <img src="https://images.unsplash.com/photo-1609630875171-b1321377ee65?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Шлем Nolan">
        </div>
        <div class="product-card-info">
          <h3 class="product-card-title">Шлем Nolan N100</h3>
          <p class="product-card-price">18 900 ₽</p>
          <div class="product-card-actions">
            <button class="product-card-add-to-cart">В корзину</button>
          </div>
        </div>
      </div>

      <!-- Товар 3 -->
      <div class="product-card">
        <div class="product-image">
          <img src="https://images.unsplash.com/photo-1571068316343-3a1c16c407e3?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Шлем HJC">
        </div>
        <div class="product-card-info">
          <h3 class="product-card-title">Шлем HJC i90</h3>
          <p class="product-card-price">16 700 ₽</p>
          <div class="product-card-actions">
            <button class="product-card-add-to-cart">В корзину</button>
          </div>
        </div>
      </div>

      <!-- Товар 4 -->
      <div class="product-card">
        <div class="product-image">
          <img src="https://images.unsplash.com/photo-1558618047-3c8c76ca7d13?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Шлем LS2">
        </div>
        <div class="product-card-info">
          <h3 class="product-card-title">Шлем LS2 Valiant</h3>
          <p class="product-card-price">14 200 ₽</p>
          <div class="product-card-actions">
            <button class="product-card-add-to-cart">В корзину</button>
          </div>
        </div>
      </div>
    </div>
  </div>

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
  </div>
</template>

<style scoped>
  /* Общие стили */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.product-container {
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

/* Хлебные крошки */
.breadcrumbs {
  padding: 1.5rem 0;
  color: #aaa;
  font-size: 0.9rem;
}

.breadcrumbs a {
  color: #ff4500;
  text-decoration: none;
  transition: color 0.3s;
}

.breadcrumbs a:hover {
  color: #ff5500;
}

.breadcrumbs span {
  margin: 0 0.5rem;
}

/* Карточка товара */
.product-detail {
  display: flex;
  gap: 3rem;
  padding: 2rem 0;
}

.product-gallery {
  flex: 1;
}

.main-image {
  background-color: #000;
  border-radius: 8px;
  overflow: hidden;
  margin-bottom: 1rem;
  border: 1px solid #333;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 400px;
}

.main-image img {
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
}

.image-thumbnails {
  display: flex;
  gap: 0.5rem;
}

.thumbnail {
  width: 80px;
  height: 80px;
  background-color: #000;
  border-radius: 4px;
  overflow: hidden;
  cursor: pointer;
  border: 1px solid #333;
  transition: border-color 0.3s;
  display: flex;
  justify-content: center;
  align-items: center;
}

.thumbnail:hover, .thumbnail.active {
  border-color: #ff4500;
}

.thumbnail img {
  max-width: 100%;
  max-height: 100%;
  object-fit: cover;
}

.product-info {
  flex: 1;
}

.product-category {
  color: #ff4500;
  font-size: 0.9rem;
  text-transform: uppercase;
  letter-spacing: 1px;
  margin-bottom: 0.5rem;
}

.product-title {
  font-size: 2rem;
  margin-bottom: 1rem;
  color: #f0f0f0;
}

.product-rating {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  margin-bottom: 1.5rem;
}

.stars {
  color: #ff4500;
}

.rating-count {
  color: #aaa;
  font-size: 0.9rem;
}

.product-price {
  font-size: 2.2rem;
  font-weight: bold;
  color: #ff4500;
  margin-bottom: 1.5rem;
}

.product-description {
  color: #aaa;
  margin-bottom: 2rem;
  line-height: 1.6;
}

.product-features {
  margin-bottom: 2rem;
}

.features-title {
  font-size: 1.2rem;
  margin-bottom: 1rem;
  color: #f0f0f0;
}

.features-list {
  list-style: none;
}

.features-list li {
  margin-bottom: 0.5rem;
  padding-left: 1.5rem;
  position: relative;
}

.features-list li:before {
  content: '•';
  color: #ff4500;
  position: absolute;
  left: 0;
}

.product-options {
  margin-bottom: 2rem;
}

.option-title {
  font-size: 1.1rem;
  margin-bottom: 1rem;
  color: #f0f0f0;
}

.size-options {
  display: flex;
  gap: 0.5rem;
  margin-bottom: 1.5rem;
}

.size-option {
  padding: 0.7rem 1.2rem;
  background-color: #1a1a1a;
  border: 1px solid #333;
  border-radius: 4px;
  cursor: pointer;
  transition: all 0.3s;
  font-weight: 500;
}

.size-option:hover {
  border-color: #ff4500;
  color: #ff4500;
}

.size-option.active {
  background-color: #ff4500;
  color: #000;
  border-color: #ff4500;
}

.color-options {
  display: flex;
  gap: 0.5rem;
  margin-bottom: 1.5rem;
}

.color-option {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  cursor: pointer;
  border: 2px solid transparent;
  transition: border-color 0.3s;
}

.color-option:hover {
  border-color: #ff4500;
}

.color-option.active {
  border-color: #ff4500;
}

.color-black {
  background-color: #000;
}

.color-red {
  background-color: #ff4500;
}

.color-white {
  background-color: #f0f0f0;
}

.color-blue {
  background-color: #1e90ff;
}

.product-actions {
  display: flex;
  gap: 1rem;
  margin-bottom: 2rem;
}

.quantity-selector {
  display: flex;
  align-items: center;
  background-color: #1a1a1a;
  border-radius: 4px;
  border: 1px solid #333;
  overflow: hidden;
}

.quantity-btn {
  padding: 0.8rem 1rem;
  background-color: transparent;
  color: #f0f0f0;
  border: none;
  cursor: pointer;
  transition: background-color 0.3s;
}

.quantity-btn:hover {
  background-color: #ff4500;
  color: #000;
}

.quantity-value {
  padding: 0 1rem;
  min-width: 50px;
  text-align: center;
}

.add-to-cart {
  flex: 1;
  padding: 0.8rem 1.5rem;
  background-color: #ff4500;
  color: #000;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-weight: bold;
  transition: background-color 0.3s;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-size: 1rem;
}

.add-to-cart:hover {
  background-color: #ff5500;
}

.buy-now {
  flex: 1;
  padding: 0.8rem 1.5rem;
  background-color: transparent;
  color: #ff4500;
  border: 2px solid #ff4500;
  border-radius: 4px;
  cursor: pointer;
  font-weight: bold;
  transition: all 0.3s;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-size: 1rem;
}

.buy-now:hover {
  background-color: #ff4500;
  color: #000;
}

.product-meta {
  display: flex;
  gap: 2rem;
  color: #aaa;
  font-size: 0.9rem;
  border-top: 1px solid #333;
  padding-top: 1.5rem;
}

.meta-item {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

/* Табы с дополнительной информацией */
.product-tabs {
  margin: 3rem 0;
}

.tabs-header {
  display: flex;
  border-bottom: 1px solid #333;
}

.tab {
  padding: 1rem 2rem;
  background-color: transparent;
  color: #aaa;
  border: none;
  cursor: pointer;
  transition: all 0.3s;
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: 1px;
  position: relative;
}

.tab:hover {
  color: #ff4500;
}

.tab.active {
  color: #ff4500;
}

.tab.active:after {
  content: '';
  position: absolute;
  bottom: -1px;
  left: 0;
  width: 100%;
  height: 3px;
  background-color: #ff4500;
}

.tab-content {
  padding: 2rem 0;
  display: none;
}

.tab-content.active {
  display: block;
}

.specs-table {
  width: 100%;
  border-collapse: collapse;
}

.specs-table tr {
  border-bottom: 1px solid #333;
}

.specs-table td {
  padding: 1rem 0;
}

.specs-table td:first-child {
  font-weight: 500;
  width: 30%;
}

.reviews-list {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.review {
  padding-bottom: 2rem;
  border-bottom: 1px solid #333;
}

.review:last-child {
  border-bottom: none;
}

.review-header {
  display: flex;
  justify-content: space-between;
  margin-bottom: 1rem;
}

.review-author {
  font-weight: 500;
}

.review-date {
  color: #aaa;
  font-size: 0.9rem;
}

.review-rating {
  color: #ff4500;
  margin-bottom: 0.5rem;
}

/* Похожие товары */
.related-products {
  margin: 3rem 0;
}

.section-title {
  font-size: 1.8rem;
  margin-bottom: 2rem;
  color: #f0f0f0;
  text-transform: uppercase;
  letter-spacing: 1px;
  position: relative;
}

.section-title:after {
  content: '';
  display: block;
  width: 80px;
  height: 3px;
  background-color: #ff4500;
  margin-top: 10px;
}

.products-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
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
  height: 200px;
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

.product-card-info {
  padding: 1.5rem;
}

.product-card-title {
  font-size: 1.1rem;
  margin-bottom: 0.5rem;
  color: #f0f0f0;
}

.product-card-price {
  font-size: 1.3rem;
  font-weight: bold;
  color: #ff4500;
  margin-bottom: 1rem;
}

.product-card-actions {
  display: flex;
  gap: 0.5rem;
}

.product-card-add-to-cart {
  flex: 1;
  padding: 0.7rem;
  background-color: #ff4500;
  color: #000;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-weight: bold;
  transition: background-color 0.3s;
  text-transform: uppercase;
  font-size: 0.8rem;
}

.product-card-add-to-cart:hover {
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
@media (max-width: 968px) {
  .product-detail {
    flex-direction: column;
  }

  .product-gallery, .product-info {
    width: 100%;
  }
}

@media (max-width: 768px) {
  .header-content {
    flex-direction: column;
    text-align: center;
  }

  nav ul {
    margin-top: 1rem;
    justify-content: center;
    flex-wrap: wrap;
  }

  nav ul li {
    margin: 0.5rem;
  }

  .product-actions {
    flex-direction: column;
  }

  .tabs-header {
    flex-wrap: wrap;
  }

  .footer-content {
    flex-direction: column;
  }
}

@media (max-width: 480px) {
  .products-grid {
    grid-template-columns: 1fr;
  }

  .size-options, .color-options {
    flex-wrap: wrap;
  }
}
</style>
