---
layout: default
---
# Порядок роботи
{: .text-center}

## Крок 0: Підготування {% include ref_link.liquid %}

Перед початком роботи з&nbsp;{% include bot_link.liquid %}
потрібно зареєструватися у&nbsp;сервісі {% include ref_link.liquid %}.

Там додати [торгову точку](https://youtu.be/vFiIGkTwwe0){:target="_blank"},
[створити касу](https://youtu.be/DiDsXCKEnNw){:target="_blank"} та
[зареєструвати касира](https://youtu.be/RZeBTGeFr0I){:target="_blank"}.

Далі слід завантажити ЕЦП касира у&nbsp;[хмарне сховище](https://fb.watch/alieJ_AHfc/){:target="_blank"}.
Підійде будь який діючий електронний підпис або електронна печатка вашого ФОП.

> ### Зверніть увагу!
> Кожен з&nbsp;найманих працівників повинен мати свій особистий цифровий підпис чи печатку.

Обов’язково слід заповнити позиції товарів чи послуг (розділ «Товари»), 
щоб вони відображались у&nbsp;боті для&nbsp;зручності створення чеку.

> ### Увага!
> Наразі {% include bot_link.liquid %} має обмеження у&nbsp;100 позицій,
> тобто бот відобразить лише перші 100 з&nbsp;них.

Інформація, що необхідна для&nbsp;подальшої роботи через {% include bot_link.liquid %}:
* Ключ ліцензії каси (розділ «Каси»)
* Пін-код касира (розділ «Касири»)

## Крок 1: Додавання каси

Після того, як у&nbsp;{% include ref_link.liquid %} усе налаштовано,
слід прив’язати його до&nbsp;{% include bot_link.liquid %}.

Спочатку прив’язуємо касу натиснувши «Додати касу» та ввівши ключ ліцензії каси,
який можна взяти у&nbsp;розділі «Каси».

{% include img.liquid src="/assets/images/step_1_1.jpg" group="step_1" %}
{% include img.liquid src="/assets/images/step_1_2.jpg" group="step_1" %}
{% include img.liquid src="/assets/images/step_1_3.jpg" group="step_1" %}
{: .text-center}

## Крок 2: Перший чек

Натисніть «Створити чек». Бот спитає пін-код касира для авторизації та чи слід його запам’ятати.

{% include img.liquid src="/assets/images/step_2_1.jpg" group="step_2_1" %}
{% include img.liquid src="/assets/images/step_2_2.jpg" group="step_2_1" %}
{: .text-center}

У&nbsp;азі згоди, бот більше не&nbsp;буде питати пін-код. Відмовившись, матимете вводити його щоразу. 
Скинути збережений пін-код можна у&nbsp;налаштуваннях.

У&nbsp;разі успішної авторизації, {% include bot_link.liquid %} 
запропонує обрати одну з&nbsp;позицій. Після вибору, бот автоматично відкриє зміну та створить чек.

{% include img.liquid src="/assets/images/step_2_3.jpg" group="step_2_2" %}
{% include img.liquid src="/assets/images/step_2_4.jpg" group="step_2_2" %}
{: .text-center}

Ви отримаєте:
* QR-код чека, що можна показати клієнтові
* Посилання, за&nbsp;яким чек можна знайти на&nbsp;[сайті ДПС](https://cabinet.tax.gov.ua/cashregs/check){:target="_blank"}
* Текст чеку, який можна скопіювати та роздрукувати у&nbsp;додатку до&nbsp;вашого принтеру

{% include img.liquid src="/assets/images/step_2_5.jpg" group="step_2_3" %}
{% include img.liquid src="/assets/images/step_2_6.jpg" group="step_2_3" %}
{: .text-center}

Тепер бот готовий створити ще один чек.

## Крок 3: Закриття зміни

Статистику зміни можна подивитись натиснувши «Показати звіт». 
Це приблизно те ж саме, що й X-звіт для касового апарату, але без створення такого звіту.

Натисканням «Закрити зміну» ініціюється закриття зміни з&nbsp;автоматичним вилученням готівки з&nbsp;віртуальної каси.
Тобто віртуальних залишків у&nbsp;касі не&nbsp;залишиться.

{% include img.liquid src="/assets/images/step_3_1.jpg" group="step_3" %}
{% include img.liquid src="/assets/images/step_3_2.jpg" group="step_3" %}
{: .text-center}

Після закриття зміни формується звіт, дані якого слід занести у&nbsp;книгу обліку доходів.
Якщо протягом однієї календарної дати видкривалися декілька змін, то для внесення у&nbsp;книгу доходів їхні підсумки сумуються.

# Налаштування
{: .text-center}

Меню налаштувань відкривається натисканням «Налаштувати».

Тут можна додати ще одну касу або керувати вже доданими. Можна видалити касу,
а&nbsp;також, якщо додано декілька кас, встановити касу за&nbsp;замовчуванням.

{% include img.liquid src="/assets/images/settings_1.jpg" group="settings_1" %}
{% include img.liquid src="/assets/images/settings_2.jpg" group="settings_1" %}
{: .text-center}

Можна скинути збережений пін-код касира, натиснувши «Забути пін-код».
Також тут можна навпаки&nbsp;&mdash; зберегти пін-код у разі, якщо ви передумали.

Також у налаштуваннях можна увімкнути розрахунок карткою.
Тоді головне меню метиме дві кнопки створення чеку: для готівкового розрахунку та безготівкового.
Відповідно зміниться звіт. Він матиме окремі підсумки для готівки та картки, а&nbsp;також їхню суму.

{% include img.liquid src="/assets/images/settings_3.jpg" group="settings_2" %}
{% include img.liquid src="/assets/images/settings_4.jpg" group="settings_2" %}
{: .text-center}
