<p align="center">
  <a href="https://t.me/example_store_bot"><img src="data/assets/logo.png" alt="ShopBot"></a>
</p>

Это пример Telegram shopbot. Это простой и, самое главное, эффективный способ оформить заказ, не выходя из своего любимого мессенджера

## Что он может сделать?

1. `/start` - запустить бота и выбрать режим (пользователь/администратор).

2. `/menu` - перейти к меню.

3. `/sos` - задать вопрос администратору.

## Menu

Пользовательское меню выглядит следующим образом:

![User Menu](data/assets/4.png)

## Каталог

Каталог состоит из товаров, отсортированных по категориям. Пользователи могут добавлять товары в корзину, а администратор полностью контролирует управление каталогом (добавление/удаление).

## Корзина

Процесс оформления заказа выглядит следующим образом: пользователь заходит в `🛍️ Каталог`, выбирает нужную категорию, выбирает товары и нажимает кнопку `🛒 Корзина`.

![cart](data/assets/5.png)

---

Затем, убедившись, что все на месте, перейдите к оформлению заказа, нажав кнопку `📦 Оформить заказ`.

![checkout](data/assets/6.png)

## Добавление товара

Чтобы добавить товар, выберите категорию и нажмите на кнопку `➕ Добавить товар`. Затем заполните форму "название-описание-изображение-цена" и подтвердите.

![add_product](data/assets/1.png)

## Связаться с администратором

Чтобы задать вопрос администратору, просто выберите команду `/sos` command. Количество вопросов ограничено..

![sos](data/assets/7.png)

## Установка

1. Создайте виртуальное окружение:


```bash
python3 -m venv venv
source venv/scripts/activate
```

2. Установите requirements:

```bash
pip install -r requirements.txt
```

3. Заполните файл `.env`. Необходимые ключи (_\*_ - требуется всегда; _\*\*_ - требуется только в рабочей среде):

| Key                                  | Value                                                                                                                                                                                             |
| ------------------------------------ |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| BOT*TOKEN (*\*\_)                    | Чтобы получить токен бота, вам необходимо создать бота с помощью [BotFather](https://t.me/BotFather/).                                                                                            |
| ADMINS (_\*\*_)                      | Строка идентификаторов администраторов, разделенных запятыми (например, 000000000,123456789). Чтобы получить свой идентификатор в Telegram, используйте[Get My ID bot](https://t.me/getmyid_bot). |

Example:

```properties
BOT_TOKEN=YOUR_BOT_TOKEN
ADMINS=123456789,000000000
```

5. Run `app.py`:

```bash
python3 app.py
```
#   b o t  
 