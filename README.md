# Thermal Printer UI Project

---

## 🖨️ Summary

**Thermal Printer UI** is a simple, cross-platform **Python GUI application** designed to easily print text and images to **ESC/POS compatible thermal printers** over a serial (COM) port.

It offers a user-friendly interface for:
* **Custom text printing**: Adjust font size and alignment.
* **Intelligent image printing**: Automatic contrast enhancement and dithering for optimal monochrome output, maintaining aspect ratio.
* **Live image preview**: See your image before you print it.

Built with **Pillow**, **pyserial**, and **tkinter**, this project provides a straightforward solution for various thermal printing needs.

---

## 🚀 Getting Started

Follow these steps to get your Thermal Printer UI up and running.

### 🔧 Requirements

* **Python 3.8+**
* `Pillow` library
* `pyserial` library
* An **ESC/POS-compatible thermal printer** (supporting GS v 0 / raster commands)
* A **COM port** for connection (default: `COM3`, can be adjusted in `main.py`)

### 📦 Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Timur1616/thermal-printer-ui.git](https://github.com/Timur1616/thermal-printer-ui.git)
    cd thermal-printer-ui
    ```

2.  **Install dependencies:**
    ```bash
    pip install Pillow
    pip install pyserial
    ```

### 🏃 How to Run

1.  **Adjust COM Port (if needed):**
    Open `main.py` and modify the `COM_PORT` variable to match your printer's serial port (e.g., `'COM1'`, `'COM4'`, etc.):
    ```python
    COM_PORT = 'COM3' # Change this to your printer's COM port
    ```

2.  **Run the application:**
    ```bash
    python main.py
    ```

---

## ✨ Features

* **Text Printing:**
    * Input multi-line text.
    * Select custom font sizes.
    * Choose text alignment (left, center, right).
    * Automatic calculation of text height.
* **Image Printing:**
    * Convert images to grayscale.
    * Apply automatic contrast adjustment.
    * Resize images to fit the printer's `PRINTER_WIDTH` (default 384px) while preserving aspect ratio.
    * Convert to 1-bit (dithered) for optimal thermal printing.
    * Send images using the `ESC/POS GS v 0` command.
* **Graphical User Interface (GUI):**
    * Simple and intuitive Tkinter layout.
    * Text input field.
    * File dialog for image selection.
    * **Live image preview** below the buttons.
    * Informative error/success dialogs using `messagebox`.

---

## 💡 TODO Ideas

* [ ] COM port auto-detection.
* [ ] RGB LED control from GUI.
* [ ] Language selection within the UI.
* [ ] Save & export last prints.
* [ ] Configurable printer width from the GUI.

---

## 🌐 Languages

The project documentation and UI elements (where applicable) support:
* 🇬🇧 English
* 🇺🇦 Українська
* 🇷🇺 Русский

---

## 👤 Author

**Timur1616**

---

---

# Термопринтер UI Проєкт

---

## 🖨️ Опис

**Термопринтер UI** — це простий, кросплатформний **Python GUI-додаток**, розроблений для легкого друку тексту та зображень на **термопринтерах, сумісних з ESC/POS**, через послідовний (COM) порт.

Він пропонує зручний інтерфейс для:
* **Друку тексту з налаштуваннями**: Регулювання розміру шрифту та вирівнювання.
* **Інтелектуального друку зображень**: Автоматичне покращення контрасту та дизеринг для оптимального монохромного виведення, зі збереженням співвідношення сторін.
* **Попереднього перегляду зображення в реальному часі**: Переглядайте зображення перед друком.

Створений за допомогою **Pillow**, **pyserial** та **tkinter**, цей проєкт надає просте рішення для різноманітних потреб термодруку.

---

## 🚀 Початок Роботи

Виконайте ці кроки, щоб запустити Термопринтер UI.

### 🔧 Вимоги

* **Python 3.8+**
* Бібліотека `Pillow`
* Бібліотека `pyserial`
* **Термопринтер, сумісний з ESC/POS** (підтримка команд GS v 0 / растрових)
* **COM-порт** для підключення (за замовчуванням: `COM3`, можна змінити в `main.py`)

### 📦 Встановлення

1.  **Клонуйте репозиторій:**
    ```bash
    git clone [https://github.com/Timur1616/thermal-printer-ui.git](https://github.com/Timur1616/thermal-printer-ui.git)
    cd thermal-printer-ui
    ```

2.  **Встановіть залежності:**
    ```bash
    pip install Pillow
    pip install pyserial
    ```

### 🏃 Як Запустити

1.  **Налаштуйте COM-порт (за потреби):**
    Відкрийте `main.py` та змініть змінну `COM_PORT` відповідно до послідовного порту вашого принтера (наприклад, `'COM1'`, `'COM4'`, тощо):
    ```python
    COM_PORT = 'COM3' # Змініть це на COM-порт вашого принтера
    ```

2.  **Запустіть додаток:**
    ```bash
    python main.py
    ```

---

## ✨ Можливості

* **Друк Тексту:**
    * Введення багаторядкового тексту.
    * Вибір довільного розміру шрифту.
    * Вирівнювання тексту (ліворуч, по центру, праворуч).
    * Автоматичний розрахунок висоти тексту.
* **Друк Зображень:**
    * Перетворення зображень у градації сірого.
    * Застосування автоматичного налаштування контрасту.
    * Зміна розміру зображень для відповідності ширині принтера (`PRINTER_WIDTH`, за замовчуванням 384px) зі збереженням співвідношення сторін.
    * Перетворення у 1-бітний формат (дизеринг) для оптимального термодруку.
    * Надсилання зображень за допомогою команди `ESC/POS GS v 0`.
* **Графічний Інтерфейс Користувача (GUI):**
    * Простий та інтуїтивно зрозумілий макет Tkinter.
    * Поле введення тексту.
    * Діалогове вікно вибору файлу зображення.
    * **Попередній перегляд зображення** під кнопками.
    * Інформативні діалоги помилок/успіху за допомогою `messagebox`.

---

## 💡 Ідеї для TODO

* [ ] Автоматичне визначення COM-порту.
* [ ] Керування RGB LED з GUI.
* [ ] Вибір мови в інтерфейсі.
* [ ] Збереження та експорт останніх відбитків.
* [ ] Конфігурація ширини принтера з GUI.

---

## 🌐 Мови

Документація проєкту та елементи інтерфейсу (де застосовно) підтримують:
* 🇬🇧 English
* 🇺🇦 Українська
* 🇷🇺 Русский

---

## 👤 Автор

**Timur1616**

---

---

# Проект "Термопринтер UI"

---

## 🖨️ Краткое описание

**Термопринтер UI** — это простое кроссплатформенное **графическое приложение (GUI) на Python**, разработанное для удобной печати текста и изображений на **термопринтерах, совместимых с ESC/POS**, через последовательный (COM) порт.

Он предлагает удобный интерфейс для:
* **Настраиваемой печати текста**: Регулировка размера шрифта и выравнивания.
* **Интеллектуальной печати изображений**: Автоматическое улучшение контраста и дизеринг для оптимального монохромного вывода, с сохранением соотношения сторон.
* **Предварительного просмотра изображения в реальном времени**: Просматривайте изображение перед печатью.

Созданный с использованием **Pillow**, **pyserial** и **tkinter**, этот проект предоставляет простое решение для различных задач термопечати.

---

## 🚀 Начало работы

Выполните следующие шаги, чтобы запустить "Термопринтер UI".

### 🔧 Требования

* **Python 3.8+**
* Библиотека `Pillow`
* Библиотека `pyserial`
* **Термопринтер, совместимый с ESC/POS** (поддерживающий команды GS v 0 / растровые)
* **COM-порт** для подключения (по умолчанию: `COM3`, можно настроить в `main.py`)

### 📦 Установка

1.  **Клонируйте репозиторий:**
    ```bash
    git clone [https://github.com/Timur1616/thermal-printer-ui.git](https://github.com/Timur1616/thermal-printer-ui.git)
    cd thermal-printer-ui
    ```

2.  **Установите зависимости:**
    ```bash
    pip install Pillow
    pip install pyserial
    ```

### 🏃 Как запустить

1.  **Настройте COM-порт (при необходимости):**
    Откройте `main.py` и измените переменную `COM_PORT` в соответствии с последовательным портом вашего принтера (например, `'COM1'`, `'COM4'` и т.д.):
    ```python
    COM_PORT = 'COM3' # Измените это на COM-порт вашего принтера
    ```

2.  **Запустите приложение:**
    ```bash
    python main.py
    ```

---

## ✨ Возможности

* **Печать Текста:**
    * Ввод многострочного текста.
    * Выбор пользовательского размера шрифта.
    * Выравнивание текста (по левому краю, по центру, по правому краю).
    * Автоматический расчет высоты текста.
* **Печать Изображений:**
    * Преобразование изображений в оттенки серого.
    * Применение автоматической настройки контраста.
    * Изменение размера изображений для соответствия ширине принтера (`PRINTER_WIDTH`, по умолчанию 384px) с сохранением соотношения сторон.
    * Преобразование в 1-битный формат (дизеринг) для оптимальной термопечати.
    * Отправка изображений с помощью команды `ESC/POS GS v 0`.
* **Графический Пользовательский Интерфейс (GUI):**
    * Простой и интуитивно понятный макет Tkinter.
    * Поле ввода текста.
    * Диалоговое окно для выбора файла изображения.
    * **Предварительный просмотр изображения** под кнопками.
    * Информативные диалоги об ошибках/успехе с использованием `messagebox`.

---

## 💡 Идеи для TODO

* [ ] Автоматическое определение COM-порта.
* [ ] Управление RGB LED из GUI.
* [ ] Выбор языка в интерфейсе.
* [ ] Сохранение и экспорт последних распечаток.
* [ ] Настраиваемая ширина принтера из GUI.

---

## 🌐 Языки

Документация проекта и элементы интерфейса (где применимо) подходят:
* 🇬🇧 English
* 🇺🇦 Українська
* 🇷🇺 Русский

---

## 👤 Автор

**Timur1616**
