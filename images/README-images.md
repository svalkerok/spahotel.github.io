# Інструкції з додавання зображень

## Рекомендовані зображення для сайту

Для повної візуальної копії дизайну потрібно додати наступні зображення в папку `images/`:

### Основні зображення:

1. **hero-background.jpg** - Фонове зображення для героя (1920x1080px або більше)
   - Рекомендації: Розкішний готель або курорт, теплі тони

2. **deluxe-room.jpg** - Зображення стандартного номеру (800x600px)
   - Рекомендації: Елегантний готельний номер

3. **deluxe-sea-view.jpg** - Номер з видом на море (800x600px)
   - Рекомендації: Номер з великими вікнами і видом на воду

4. **family-suite.jpg** - Сімейний номер (800x600px)
   - Рекомендації: Просторий номер з сімейною обстановкою

### Додаткові зображення:

5. **suite-gallery-1.jpg** - Перше зображення галереї (600x400px)
6. **suite-gallery-2.jpg** - Друге зображення галереї (600x400px)  
7. **suite-gallery-3.jpg** - Третє зображення галереї (600x400px)

### Іконки та логотипи:

8. **logo.png** - Логотип готелю (300x100px, прозорий фон)
9. **favicon.ico** - Іконка для браузера (32x32px)

## Як додати зображення:

1. Збережіть зображення в папку `/images/` з відповідними назвами
2. Оновіть CSS файл, замінивши градієнтні фони на реальні зображення:

```css
.hero-background {
    background-image: url('../images/hero-background.jpg');
    background-size: cover;
    background-position: center;
}

.room-image {
    background-size: cover;
    background-position: center;
}

/* Для кожної кімнати окремо */
.room-card:nth-child(1) .room-image {
    background-image: url('../images/deluxe-room.jpg');
}

.room-card:nth-child(2) .room-image {
    background-image: url('../images/deluxe-sea-view.jpg');
}

.room-card:nth-child(3) .room-image {
    background-image: url('../images/family-suite.jpg');
}
```

3. Оновіть HTML файл для додавання favicon:

```html
<link rel="icon" type="image/x-icon" href="images/favicon.ico">
```

## Рекомендовані розміри та формати:

- **Формати**: JPG для фотографій, PNG для логотипів та іконок
- **Оптимізація**: Стисніть зображення для швидшого завантаження
- **Адаптивність**: Використовуйте зображення високої роздільності для Retina дисплеїв

## Джерела зображень:

1. **Оригінальний Canva дизайн**: Експортуйте зображення з Canva дизайну
2. **Stock photos**: Unsplash, Pexels, Pixabay (безкоштовні)
3. **Premium stocks**: Shutterstock, Getty Images (платні)

## Альтернативний варіант:

Якщо зображення недоступні, поточний дизайн використовує CSS градієнти та емодзі іконки, які створюють професійний вигляд і без реальних фотографій.