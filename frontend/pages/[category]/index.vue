<script setup lang="ts">

</script>

<template>
  <div class="catalog-container">
  <header>
    <div class="container header-content">
      <div class="logo">Moto<span>Store</span></div>
      <nav>
        <ul>
          <li><a href="#">Главная</a></li>
          <li><a href="#" style="color: #ff4500;">Каталог</a></li>
          <li><a href="#">Экипировка</a></li>
          <li><a href="#">Запчасти</a></li>
          <li><a href="#">Аксессуары</a></li>
          <li class="cart-icon">
            Корзина
            <span class="cart-count">0</span>
          </li>
        </ul>
      </nav>
    </div>
  </header>

  <!-- Хлебные крошки -->
  <div class="container breadcrumbs">
    <a href="#">Главная</a> <span>></span> <a href="#">Каталог</a> <span>></span> <span>Все товары</span>
  </div>

  <!-- Основной контент каталога -->
  <div class="container catalog">
    <!-- Боковая панель с фильтрами -->
    <aside class="filters">
      <div class="filter-section">
        <h3 class="filter-title">Категории</h3>
        <div class="filter-options">
          <div class="filter-option">
            <input type="checkbox" id="category-helmets" checked>
            <label for="category-helmets">Шлемы</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="category-jackets" checked>
            <label for="category-jackets">Куртки</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="category-gloves" checked>
            <label for="category-gloves">Перчатки</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="category-exhaust" checked>
            <label for="category-exhaust">Выхлопные системы</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="category-parts" checked>
            <label for="category-parts">Запчасти</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="category-accessories" checked>
            <label for="category-accessories">Аксессуары</label>
          </div>
        </div>
      </div>

      <div class="filter-section">
        <h3 class="filter-title">Цена</h3>
        <div class="price-range">
          <div class="price-inputs">
            <input type="number" placeholder="От" value="0">
            <input type="number" placeholder="До" value="50000">
          </div>
        </div>
      </div>

      <div class="filter-section">
        <h3 class="filter-title">Бренд</h3>
        <div class="filter-options">
          <div class="filter-option">
            <input type="checkbox" id="brand-agv" checked>
            <label for="brand-agv">AGV</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="brand-alpinestars" checked>
            <label for="brand-alpinestars">Alpinestars</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="brand-yoshimura" checked>
            <label for="brand-yoshimura">Yoshimura</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="brand-dainese" checked>
            <label for="brand-dainese">Dainese</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="brand-shark" checked>
            <label for="brand-shark">Shark</label>
          </div>
        </div>
      </div>

      <div class="filter-section">
        <h3 class="filter-title">Размер</h3>
        <div class="filter-options">
          <div class="filter-option">
            <input type="checkbox" id="size-s">
            <label for="size-s">S</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="size-m" checked>
            <label for="size-m">M</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="size-l" checked>
            <label for="size-l">L</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="size-xl">
            <label for="size-xl">XL</label>
          </div>
          <div class="filter-option">
            <input type="checkbox" id="size-xxl">
            <label for="size-xxl">XXL</label>
          </div>
        </div>
      </div>

      <button class="apply-filters">Применить фильтры</button>
    </aside>

    <!-- Секция товаров -->
    <section class="products-grid">
      <div class="products-header">
        <h2>Все товары</h2>
        <div class="products-count">Найдено 12 товаров</div>
        <div class="sort-options">
          <span>Сортировка:</span>
          <select>
            <option>По популярности</option>
            <option>По цене (сначала дешевые)</option>
            <option>По цене (сначала дорогие)</option>
            <option>По новизне</option>
          </select>
        </div>
      </div>

      <div class="product-grid">
        <!-- Товар 1 -->
        <div class="product-card">
          <div class="product-image">
            <img src="https://images.unsplash.com/photo-1628149330013-90e8a987969b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Мотошлем">
          </div>
          <div class="product-info">
            <div class="product-category">Шлемы</div>
            <h3 class="product-title">Шлем AGV Sport Modular</h3>
            <p class="product-price">24 999 ₽</p>
            <p class="product-description">Спортивный модульный шлем с системой вентиляции и защитой от запотевания</p>
            <div class="product-actions">
              <button class="add-to-cart">В корзину</button>
              <button class="view-details">Подробнее</button>
            </div>
          </div>
        </div>

        <!-- Товар 2 -->
        <div class="product-card">
          <div class="product-image">
            <img src="https://images.unsplash.com/photo-1628149330106-6433a66d4769?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Куртка кожаная">
          </div>
          <div class="product-info">
            <div class="product-category">Куртки</div>
            <h3 class="product-title">Кожаная куртка MotoStyle</h3>
            <p class="product-price">18 500 ₽</p>
            <p class="product-description">Классическая кожаная куртка с защитой на плечах и локтях</p>
            <div class="product-actions">
              <button class="add-to-cart">В корзину</button>
              <button class="view-details">Подробнее</button>
            </div>
          </div>
        </div>

        <!-- Товар 3 -->
        <div class="product-card">
          <div class="product-image">
            <img src="https://images.unsplash.com/photo-1571068316343-3a1c16c407e3?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Перчатки">
          </div>
          <div class="product-info">
            <div class="product-category">Перчатки</div>
            <h3 class="product-title">Перчатки Alpinestars GP Pro</h3>
            <p class="product-price">7 800 ₽</p>
            <p class="product-description">Спортивные перчатки с защитой костяшек и карбоновыми вставками</p>
            <div class="product-actions">
              <button class="add-to-cart">В корзину</button>
              <button class="view-details">Подробнее</button>
            </div>
          </div>
        </div>

        <!-- Товар 4 -->
        <div class="product-card">
          <div class="product-image">
            <img src="https://images.unsplash.com/photo-1558618047-3c8c76ca7d13?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Выхлопная система">
          </div>
          <div class="product-info">
            <div class="product-category">Выхлопные системы</div>
            <h3 class="product-title">Выхлопная система Yoshimura</h3>
            <p class="product-price">42 500 ₽</p>
            <p class="product-description">Титановая выхлопная система для увеличения мощности и улучшения звука</p>
            <div class="product-actions">
              <button class="add-to-cart">В корзину</button>
              <button class="view-details">Подробнее</button>
            </div>
          </div>
        </div>

        <!-- Товар 5 -->
        <div class="product-card">
          <div class="product-image">
            <img src="https://images.unsplash.com/photo-1609630875171-b1321377ee65?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Мотоочки">
          </div>
          <div class="product-info">
            <div class="product-category">Аксессуары</div>
            <h3 class="product-title">Защитные очки MotoVision</h3>
            <p class="product-price">3 200 ₽</p>
            <p class="product-description">Спортивные защитные очки с противоударными линзами</p>
            <div class="product-actions">
              <button class="add-to-cart">В корзину</button>
              <button class="view-details">Подробнее</button>
            </div>
          </div>
        </div>

        <!-- Товар 6 -->
        <div class="product-card">
          <div class="product-image">
            <img src="https://images.unsplash.com/photo-1558618667-3404e57f3b33?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" alt="Мотоботы">
          </div>
          <div class="product-info">
            <div class="product-category">Обувь</div>
            <h3 class="product-title">Мотоботы Dainese Torque</h3>
            <p class="product-price">15 700 ₽</p>
            <p class="product-description">Высокие мотоботы с защитой голеностопа и подошвой повышенного сцепления</p>
            <div class="product-actions">
              <button class="add-to-cart">В корзину</button>
              <button class="view-details">Подробнее</button>
            </div>
          </div>
        </div>
      </div>

      <!-- Пагинация -->
      <div class="pagination">
        <button class="active">1</button>
        <button>2</button>
        <button>3</button>
        <button>...</button>
        <button>10</button>
      </div>
    </section>
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

.catalog-container {
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
  padding: 1rem 0;
  color: #aaa;
  font-size: 0.9rem;
}

.breadcrumbs a {
  color: #ff4500;
  text-decoration: none;
}

.breadcrumbs span {
  margin: 0 0.5rem;
}

/* Основной контент каталога */
.catalog {
  display: flex;
  gap: 2rem;
  padding: 2rem 0;
}

/* Боковая панель с фильтрами */
.filters {
  flex: 0 0 280px;
  background-color: #1a1a1a;
  border-radius: 8px;
  padding: 1.5rem;
  height: fit-content;
  border: 1px solid #333;
}

.filter-section {
  margin-bottom: 2rem;
  border-bottom: 1px solid #333;
  padding-bottom: 1.5rem;
}

.filter-section:last-child {
  border-bottom: none;
  margin-bottom: 0;
}

.filter-title {
  font-size: 1.2rem;
  margin-bottom: 1rem;
  color: #ff4500;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.filter-options {
  display: flex;
  flex-direction: column;
  gap: 0.8rem;
}

.filter-option {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.filter-option input {
  accent-color: #ff4500;
}

.filter-option label {
  cursor: pointer;
}

.price-range {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.price-inputs {
  display: flex;
  gap: 0.5rem;
}

.price-inputs input {
  flex: 1;
  padding: 0.5rem;
  background-color: #000;
  border: 1px solid #333;
  border-radius: 4px;
  color: #f0f0f0;
}

.apply-filters {
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
  margin-top: 1rem;
}

.apply-filters:hover {
  background-color: #ff5500;
}

/* Секция товаров */
.products-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 2rem;
}

.products-count {
  color: #aaa;
}

.sort-options {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.sort-options select {
  padding: 0.5rem;
  background-color: #000;
  border: 1px solid #333;
  border-radius: 4px;
  color: #f0f0f0;
}

.products-grid {
  flex: 1;
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

.product-category {
  color: #ff4500;
  font-size: 0.8rem;
  text-transform: uppercase;
  letter-spacing: 1px;
  margin-bottom: 0.5rem;
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

.product-actions {
  display: flex;
  gap: 0.5rem;
}

.add-to-cart {
  flex: 1;
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

.view-details {
  padding: 0.8rem 1rem;
  background-color: transparent;
  color: #ff4500;
  border: 1px solid #ff4500;
  border-radius: 4px;
  cursor: pointer;
  font-weight: bold;
  transition: all 0.3s;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.view-details:hover {
  background-color: #ff4500;
  color: #000;
}

/* Пагинация */
.pagination {
  display: flex;
  justify-content: center;
  margin-top: 3rem;
  gap: 0.5rem;
}

.pagination button {
  padding: 0.5rem 1rem;
  background-color: #1a1a1a;
  color: #f0f0f0;
  border: 1px solid #333;
  border-radius: 4px;
  cursor: pointer;
  transition: all 0.3s;
}

.pagination button.active {
  background-color: #ff4500;
  color: #000;
  border-color: #ff4500;
}

.pagination button:hover:not(.active) {
  border-color: #ff4500;
  color: #ff4500;
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
  .catalog {
    flex-direction: column;
  }

  .filters {
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

  .products-header {
    flex-direction: column;
    align-items: flex-start;
    gap: 1rem;
  }

  .footer-content {
    flex-direction: column;
  }
}

@media (max-width: 480px) {
  .product-grid {
    grid-template-columns: 1fr;
  }

  .product-actions {
    flex-direction: column;
  }
}
</style>
