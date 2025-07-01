Thermal Printer UI Project
🖨️ Summary
Thermal Printer UI is a simple, cross-platform Python GUI application designed to easily print text and images to ESC/POS compatible thermal printers over a serial (COM) port.

It offers a user-friendly interface for:

Custom text printing: Adjust font size and alignment.

Intelligent image printing: Automatic contrast enhancement and dithering for optimal monochrome output, maintaining aspect ratio.

Live image preview: See your image before you print it.

Built with Pillow, pyserial, and tkinter, this project provides a straightforward solution for various thermal printing needs.

🚀 Getting Started
Follow these steps to get your Thermal Printer UI up and running.

🔧 Requirements
Python 3.8+

Pillow library

pyserial library

An ESC/POS-compatible thermal printer (supporting GS v 0 / raster commands)

A COM port for connection (default: COM3, can be adjusted in main.py)

📦 Installation
Clone the repository:

Bash

git clone https://github.com/Timur1616/thermal-printer-ui.git
cd thermal-printer-ui
Install dependencies:

Bash

pip install -r requirements.txt
(If requirements.txt is not present, you can install them manually: pip install Pillow pyserial)

🏃 How to Run
Adjust COM Port (if needed):
Open main.py and modify the COM_PORT variable to match your printer's serial port (e.g., 'COM1', 'COM4', etc.):

Python

COM_PORT = 'COM3' # Change this to your printer's COM port
Run the application:

Bash

python main.py
✨ Features
Text Printing:

Input multi-line text.

Select custom font sizes.

Choose text alignment (left, center, right).

Automatic calculation of text height.

Image Printing:

Convert images to grayscale.

Apply automatic contrast adjustment.

Resize images to fit the printer's PRINTER_WIDTH (default 384px) while preserving aspect ratio.

Convert to 1-bit (dithered) for optimal thermal printing.

Send images using the ESC/POS GS v 0 command.

Graphical User Interface (GUI):

Simple and intuitive Tkinter layout.

Text input field.

File dialog for image selection.

Live image preview below the buttons.

Informative error/success dialogs using messagebox.

💡 TODO Ideas
[ ] COM port auto-detection.

[ ] RGB LED control from GUI.

[ ] Language selection within the UI.

[ ] Save & export last prints.

[ ] Configurable printer width from the GUI.

🌐 Languages
The project documentation and UI elements (where applicable) support:

🇬🇧 English

🇺🇦 Українська

🇷🇺 Русский

👤 Author
Timur1616

