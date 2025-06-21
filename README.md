WhatsApp Desktop Number Checker

This is a Python GUI tool that automates the process of verifying whether a phone number is registered on WhatsApp using the WhatsApp Desktop application. It uses GUI automation through pyautogui, and a simple tkinter-based interface for input/output file selection and progress monitoring.

🚀 Features

✅ GUI with file picker for input and export

✅ Progress bar to visualize verification status

✅ Auto-detect invalid WhatsApp numbers using screen detection

✅ Begins with clicking the WhatsApp Desktop "New Chat" button (via start_button.png)

✅ Threaded to avoid freezing the GUI

✅ Generates log file with true/false results for each number

✅ Verifies using WhatsApp Desktop (no API required)

🖥️ How It Works

Launch WhatsApp Desktop and make sure it is open and logged in.

Open the script and select your input file (phone numbers).

Select your export output file.

Click Start Process.

The script automates the following:

Clicks the "New Chat" button (start_button.png)

Opens phone number entry via phone_button.png

Selects country (Canada)

Inputs number

Waits for WhatsApp to validate

Checks screen for invalid_popup.png

Saves number if valid

📦 Requirements

Python 3.6+

WhatsApp Desktop (must be installed and logged in)

📥 Install Python Libraries

pip install pyautogui pillow opencv-python pyperclip

Note: tkinter is included with most Python installations.

📁 Folder Contents

File

Description

whatsapp_checker.py

Main application script

start_button.png

Screenshot of the WhatsApp "New Chat" button

phone_button.png

Screenshot of the phone number input button

country_dropdown.png

Screenshot of the country dropdown list

canada.png

Screenshot of the Canada selection

invalid_popup.png

Screenshot showing WhatsApp's "not on WhatsApp" error

numbers.txt

Sample input file with phone numbers

output.txt

Output file with verified numbers

log.txt

Log of all checked numbers with status

📌 Input Format

File: numbers.txt

Format: One number per line

Must be international format (e.g., +19052010000)

+19052010000
+19052010001
+19052010002

📝 Output

Valid WhatsApp numbers are written to the export file (output.txt)

Log file log.txt contains all numbers with a true/false flag

+19052010001 — true
+19052010002 — false

🧠 Tips

Make sure WhatsApp Desktop is in the foreground.

Screenshots (*.png) must match your screen resolution and WhatsApp theme.

Use pyautogui.screenshot() to capture custom images if needed.

Delay values can be adjusted with time.sleep() if your PC is slower/faster.

If image matching fails, try increasing the confidence value (e.g., to 0.9).

🔐 Disclaimer

This tool does not use the WhatsApp API. It only automates mouse/keyboard and screen detection. Do not use this tool for spam or abusive purposes. Use responsibly and respect privacy laws.

📄 License

This project is licensed under the MIT License.

🙋 Contributing

Pull requests are welcome! If you'd like to contribute features or improvements:

Fork the repo

Create a new branch

Submit a PR

📧 Contact

For questions, suggestions or help, feel free to open an Issue or reach out via GitHub.

Happy verifying! ✅
