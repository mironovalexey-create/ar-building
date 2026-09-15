ПЕРВЫЙ ПРОТОТИП AR

Что здесь есть:
- index.html — WebAR-сцена на MindAR + A-Frame
- assets/target.jpg — исходное изображение, которое нужно использовать как Image Target
- assets/building.glb — ваша 3D-модель
- targets.mind — НУЖНО ПОЛУЧИТЬ НА ШАГЕ 1

ШАГ 1. Создать Image Target
1. Откройте MindAR Target Compiler:
   https://hiukim.github.io/mind-ar-js-doc/tools/compile/
2. Загрузите assets/target.jpg
3. Нажмите Start/Compile и скачайте targets.mind
4. Положите targets.mind рядом с index.html.

ШАГ 2. Запустить сайт
Камера смартфона обычно требует HTTPS. Просто открыть index.html через file:// недостаточно.

Самый простой способ для теста — любой статический HTTPS-хостинг. Например, GitHub Pages, Netlify или Cloudflare Pages.
Загрузите:
  index.html
  targets.mind
  assets/target.jpg
  assets/building.glb

После публикации откройте URL на смартфоне, разрешите камеру и наведите её на распечатанное/показанное на другом экране изображение target.jpg.

ВАЖНО
Изображение target.jpg должно быть тем же изображением, которое система видит камерой. Если оно будет существенно изменено при печати, сначала проверим качество распознавания.

МАСШТАБ
Сейчас модель рассчитана примерно на ширину, равную ширине Image Target. Это стартовое значение. Если объект окажется слишком маленьким/большим, меняем scale в index.html.
