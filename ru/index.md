---
lang: ru
ref: home
title: Табло для OBS, Streamlabs, Wirecast и Meld
description: >
  Приложение-табло для macOS с бесплатной пробной версией: счёт, таймер, удаления и статистика
  команд в спортивной трансляции через TXT-файлы для OBS, Streamlabs, Wirecast и Meld.
image: /img/scoreboard_for_mac_light.png
layout: home
permalink: /ru/
---

Полнофункциональная утилита для вывода статистики в спортивной трансляции через OBS, Streamlabs, Wirecast, Meld и другие программы для стриминга, которые поддерживают источники из текстовых файлов и изображений. Она поможет показать поверх видео онлайн-трансляции всю нужную статистику конкретной игры.

Данные записываются в TXT-файлы на диске вашего компьютера (по умолчанию — в папку «Загрузки»). Каждый файл можно добавить в программу для стриминга (источник «Текст») и наложить на любое изображение вашего табло.

<p align="center">
	<img class="header-image" alt="Главный экран ScoreBoard для Mac" src="/img/scoreboard_for_mac_light.png">
</p>

## Что табло может показывать в спортивной трансляции:
- Время (таймер или секундомер) с десятыми долями секунды
- Дополнительный таймер с двумя пресетами (например, для баскетбола)
- Голы (очки, броски) каждой команды
- Два дополнительных счётчика очков/бросков для обеих команд
- Период (тайм, четверть)
- Названия двух команд и матча
- Описания/статусы/промо двух команд и матча
- Удаления с таймерами для хоккея и похожих игр
- Жёлтые и красные карточки для футбола
- Логотипы и промо двух команд и матча

### Дополнительные возможности:
- Горячие клавиши для удобного управления
- Обмен статистикой команд местами
- Сброс статистики
- Автоматическое сохранение настроек табло
- Выбор папки для записи выходных TXT-файлов
- Увеличение счёта сразу на +1, +2, +3
- Настройка шага счётчика голов
- Управление с Touch Bar
- Суффикс для периода (1st, 2nd, 3rd)
- Ведущий ноль в счёте (01 – 05)

Впервые пользуетесь приложением? Пройдите пошаговые [инструкции по настройке](/ru/guides/) и добавьте своё первое табло в OBS.

## Отзывы пользователей

_Отзывы приведены в оригинале._

NP2003 | djithm | TofuDunk | tiivonen
--- | --- | --- | ---
I've been using this program since it was v1.0 on the OBS Forums - this is a fantastic program. | Excellent application that has all the tools required to use for your score bug in OBS. So much better than some of the paid subscriptions as long as you have the ability to create your own graphics for the scoreboard portion. Keep up the great work and I look forward to your updates! | This app has made it much easier for me to keep score during my board game streaming sessions. | Simple and easy to use. I use it for floorball streaming. Original M1 mbpro handles scoreboard and streaming 1080p 50p around 10% CPU usage.

<p align="center">
    <a href="https://apps.apple.com/app/id1579159150" title="Загрузить в Mac App Store">
        <img alt="Загрузить в Mac App Store" src="/img/MacAppStore.png">
    </a>
</p>

## Бесплатная версия ScoreBoard
**Бесплатная версия** для пробного использования: [скачайте](/free-apps/ScoreBoard-free.zip), распакуйте архив и перенесите приложение в папку «Программы».  
Бесплатная версия полностью функциональна, но вывод текста в некоторых полях ограничен.  
_Приложение нотаризовано и проверено Apple — его безопасно скачивать и использовать на Mac._
<p align="center">
    <a href="/free-apps/ScoreBoard-free.zip" title="Скачать бесплатную пробную версию">
        <img alt="Скачать бесплатную пробную версию" src="/img/free-download.png">
    </a>
</p>

## Скриншоты ScoreBoard и OBS
<p align="center">
  {% include screenshot.html name="1_main" alt="Главный экран ScoreBoard для Mac с управлением счётом и таймером" %}
  <br>
  {% include screenshot.html name="2_preferences" alt="Окно настроек ScoreBoard для Mac для настройки вывода табло" %}
  <br>
  {% include screenshot.html name="3_hotkeys" alt="Горячие клавиши и действия Touch Bar в ScoreBoard для Mac" %}
  <br>
  {% include screenshot.html name="4_txtFiles" alt="Выходные TXT-файлы ScoreBoard для Mac как текстовые источники в OBS" %}
  <br>
</p>

## Видеоинструкция
_OBS и ScoreBoard с тех пор уже несколько раз обновлялись, но настройки в видео похожи на актуальные. Видео на английском языке._

<div class="video-container">
  <iframe src="https://www.youtube.com/embed/dHj56FIE2ng?si=q62r_uccgddo2KXv&start=50" allowfullscreen></iframe>
</div>


## Пример готового табло после настройки в OBS
<p align="center">
	<img width="800" alt="Возможный шаблон табло в OBS" src="/img/output_example.jpg">
</p>

## Вопросы и ответы

**Работает ли ScoreBoard со Streamlabs, Wirecast и Meld?**  
Да. ScoreBoard записывает счёт, таймер и статистику в TXT-файлы (а промо и логотипы — в файлы изображений) на диске. Их может прочитать и показать поверх видео любая программа для стриминга, поддерживающая источники из текстовых файлов и изображений, — в том числе OBS, Streamlabs, Wirecast и Meld.

**Есть ли бесплатная версия?**  
Да, можно скачать [бесплатную пробную версию](/free-apps/ScoreBoard-free.zip), нотаризованную и проверенную Apple. Она полностью функциональна, но вывод в некоторых полях ограничен. Полная версия доступна в [Mac App Store](https://apps.apple.com/app/id1579159150).

**В каком формате ScoreBoard выводит данные?**  
Обычные TXT-файлы для текстовых значений (счёт, таймер, названия команд и т. д.) и файлы изображений для логотипов и промо-графики команд и матча. Они обновляются автоматически, пока вы управляете игрой в приложении.

**Нужны ли ScoreBoard интернет или учётная запись?**  
Нет. ScoreBoard работает полностью локально на вашем Mac и не собирает никаких данных — см. [Политику конфиденциальности](/ru/privacy/).

## Прочее
[Политика конфиденциальности](/ru/privacy/)

[Связаться с поддержкой](/ru/support/)\
*Принимаются сообщения об ошибках, пожелания и вопросы.*

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "Sports Scoreboard for OBS",
  "description": "Спортивная трансляция со статистикой на табло для OBS, Streamlabs, Wirecast, Meld и других программ.",
  "inLanguage": "ru",
  "url": "https://scoreboardmac.github.io/ru/",
  "applicationCategory": "MultimediaApplication",
  "operatingSystem": "macOS",
  "offers": {
    "@type": "Offer",
    "price": "9.99",
    "priceCurrency": "USD",
    "url": "https://apps.apple.com/app/id1579159150"
  },
  "aggregateRating": {
    "@type": "AggregateRating",
    "ratingValue": "4.5",
    "reviewCount": "44"
  },
  "review": [
    {
      "@type": "Review",
      "author": { "@type": "Person", "name": "NP2003" },
      "reviewBody": "I've been using this program since it was v1.0 on the OBS Forums - this is a fantastic program."
    },
    {
      "@type": "Review",
      "author": { "@type": "Person", "name": "djithm" },
      "reviewBody": "Excellent application that has all the tools required to use for your score bug in OBS. So much better than some of the paid subscriptions as long as you have the ability to create your own graphics for the scoreboard portion. Keep up the great work and I look forward to your updates!"
    },
    {
      "@type": "Review",
      "author": { "@type": "Person", "name": "TofuDunk" },
      "reviewBody": "This app has made it much easier for me to keep score during my board game streaming sessions."
    },
    {
      "@type": "Review",
      "author": { "@type": "Person", "name": "tiivonen" },
      "reviewBody": "Simple and easy to use. I use it for floorball streaming. Original M1 mbpro handles scoreboard and streaming 1080p 50p around 10% CPU usage."
    }
  ]
}
</script>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "inLanguage": "ru",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Работает ли ScoreBoard со Streamlabs, Wirecast и Meld?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Да. ScoreBoard записывает счёт, таймер и статистику в TXT-файлы (а промо и логотипы — в файлы изображений) на диске. Их может прочитать и показать поверх видео любая программа для стриминга, поддерживающая источники из текстовых файлов и изображений, — в том числе OBS, Streamlabs, Wirecast и Meld."
      }
    },
    {
      "@type": "Question",
      "name": "Есть ли бесплатная версия?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Да, можно скачать бесплатную пробную версию, нотаризованную и проверенную Apple. Она полностью функциональна, но вывод в некоторых полях ограничен. Полная версия доступна в Mac App Store."
      }
    },
    {
      "@type": "Question",
      "name": "В каком формате ScoreBoard выводит данные?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Обычные TXT-файлы для текстовых значений (счёт, таймер, названия команд и т. д.) и файлы изображений для логотипов и промо-графики команд и матча. Они обновляются автоматически, пока вы управляете игрой в приложении."
      }
    },
    {
      "@type": "Question",
      "name": "Нужны ли ScoreBoard интернет или учётная запись?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Нет. ScoreBoard работает полностью локально на вашем Mac и не собирает никаких данных."
      }
    }
  ]
}
</script>

<!--Styles-->
<style>
	.header-image {
		width: 500px;
	}

	@media (prefers-color-scheme: dark) {
	  .header-image {
			content: url('/img/scoreboard_for_mac_dark.png');
	  }
	}
	
	.video-container {
		width: 100%;
		max-width: 720px;
		margin: 0 auto;
	}

	.video-container iframe {
		width: 100%;
		aspect-ratio: 4/3; /* или 16/9 для широкоформатных видео */
		border: none;
	}
</style>
