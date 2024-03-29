# Лабораторна робота №1

## Тема: Адаптивна верстка статичних сторінок засобами HTML та CSS

## 1. Теоретичні відомості
Адаптивна верстка – підхід, що припускає зміну дизайну залежно від
поведінки користувача, розміру екрана, платформи і орієнтації пристрою.
Іншими словами, сторінка повинна автоматично підлаштовуватися під роздільну
здатність, змінювати розмір картинок і так далі. Це дозволяє усунути потребу в
розробці дизайну для кожного нового пристрою, що з’являється у продажу.
Адаптивну верстку можна реалізувати як засобами фреймворків, так і
безпосередньо засобами HTML та CSS із використанням CSS-запиту (query)
@media. Наступний фрагмент коду демонструє застосування цих запитів для
створення адаптивного дизайну HTML-сторінки (у наведеному прикладі стилі
CSS включені до тексту HTML-сторінки для наочності):
```html
<!DOCTYPE html>
<html>
<head>
<!-- Some meta and title here -->
<style>
/* Put some basic styles here */
.row {
width: 100%;
}
/* Large devices */
@media (min-width: 1200px) {
.col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8,
.col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 {
float: left;
border: 1px solid green;
}
.col-lg-1 {
width: 8.33%;
}
.col-lg-2 {
width: 16.66%;
}
.col-lg-3 {
width: 25%;
}
.col-lg-4 {
width: 33.33%;
}

.col-lg-5 {
width: 41.66%;
}
.col-lg-6 {
width: 50%;
}
.col-lg-7 {
width: 58.33%;
}
.col-lg-8 {
width: 66.66%;
}
.col-lg-9 {
width: 74.99%;
}
.col-lg-10 {
width: 83.33%;
}
.col-lg-11 {
width: 91.66%;
}
.col-lg-12 {
width: 100%;
}
}
/* Medium devices */
@media (min-width: 992px) and (max-width: 1199px) {
.col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8,
.col-md-9, .col-md-10, .col-md-11, .col-md-12 {
float: left;
border: 1px solid green;
}
.col-md-1 {
width: 8.33%;
}
.col-md-2 {
width: 16.66%;
}
.col-md-3 {
width: 25%;
}
.col-md-4 {
width: 33.33%;
}
.col-md-5 {
width: 41.66%;
}
.col-md-6 {
width: 50%;
}
.col-md-7 {
width: 58.33%;
}
.col-md-8 {
width: 66.66%;
}
.col-md-9 {
width: 74.99%;
}
.col-md-10 {
width: 83.33%;
}
.col-md-11 {
width: 91.66%;
}
.col-md-12 {
width: 100%;
}
}

</style>
</head>
<body>
<h1>Heading</h1>
<div class="row">
<div class="col-lg-3 col-md-6"><p>Item 1</p></div>
<div class="col-lg-3 col-md-6"><p>Item 2</p></div>
<div class="col-lg-3 col-md-6"><p>Item 3</p></div>
<div class="col-lg-3 col-md-6"><p>Item 4</p></div>
<div class="col-lg-3 col-md-6"><p>Item 5</p></div>
<div class="col-lg-3 col-md-6"><p>Item 6</p></div>
<div class="col-lg-3 col-md-6"><p>Item 7</p></div>
<div class="col-lg-3 col-md-6"><p>Item 8</p></div>
</div>
</body>
</html>
```
Властивості min-width: та max-width: у сукупності з логічними
операторами «and» та «,» (або) дозволяють встановлювати межі ширини екрану
(вікна браузера), які визначатимуть застосування того чи іншого набору стилів.
Наведений приклад спирається на модель «12-column Grid Responsive Layout».

## 2. Хід роботи
2.1. Встановіть Git та створіть на GitHub репозитарій для курсу.  
2.2. Засобами HTML та CSS (без використання фреймворків, стилі повинні
розміщуватись у окремому css-файлі) створіть сторінку, вміст якої
адаптуватиметься до розміру вікна браузера згідно макетів, наведених
у файлах desktop.png (для ширини >992px), tablet.png (для
ширини >768px та ≤992px) та mobile.png (для ширини ≤768px).
У макетах, ширину елементів слід задавати у відсотковому відношенні,
щоб вона була незмінною при зміні розмірів екрану браузера у межах
макету. Кольори, шрифти та тексти можна замінити на власні
у допустимих межах. Зверніть увагу на границі блоків тексту та
відступи між ними – вони повинні зберігатись у межах відсоткових
співвідношень блоків тексту.  
2.3. Надайте викладачеві посилання на зроблену адаптивну сторінку,
розміщену на GitHub.  
2.4. Зробіть висновки щодо виконаної роботи.  


**Мар'ян Ребега | 2020 | Івано-Франківськ**

