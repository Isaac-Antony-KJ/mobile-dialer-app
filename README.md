# 📱 Smart Mobile Call Queue & Dialer Web App

A lightweight, mobile-friendly Progressive Web App (PWA) built with HTML and JavaScript designed for streamlined outbound calling workflows (sales, surveys, customer support). It allows users to manage a dynamic call queue by selecting native phone contacts or uploading Excel/CSV spreadsheets.

## ✨ Key Features

- **📱 Native Phone Contact Picker:** Select multiple contacts directly from your Android device's contact book using the modern Contact Picker API.
- **📁 Excel & CSV Sheet Upload:** Import lists instantly from `.xlsx`, `.xls`, or `.csv` files directly in your browser. (Expects Column A for **Name** and Column B for **Phone**).
- **🔄 Smart Queue Loop:** Automatically tracks your progress, letting you step through numbers one by one.
- **⚡ Quick-Action Controls:** Features dedicated **Dial**, **Redial**, and **Next Contact** buttons to maintain high-speed calling efficiency.
- **🔒 Privacy First:** All data processing (parsing spreadsheets and managing queues) happens entirely locally on your device. No backend servers required.

## 🚀 How to Use

1. Open your hosted GitHub Pages URL in **Google Chrome on Android**.
2. Tap the Chrome menu (three dots) and select **"Add to Home screen"** or **"Install app"** for a full-screen native experience.
3. Choose either **📱 Select from Phone Contacts** or **📁 Upload Excel/CSV Sheet**.
4. Tap **📞 Dial Number** to open your native phone dialer.
5. Once the call finishes, return to the app and click **✅ Next Person** to move down the queue (or use **🔄 Redial** if needed).

## 🛠️ Built With

- **HTML5 / CSS3 / Vanilla JavaScript**
- **SheetJS (XLSX):** For client-side spreadsheet parsing.
- **Android Contact Picker API:** For secure native contact selection.

## 📄 License

This project is open-source and available for personal and commercial productivity use.
