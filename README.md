# 💰 Arc Raiders Pro Tracker

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Platform](https://img.shields.io/badge/platform-windows%20%7C%20macos-lightgrey)

A lightweight, local-first session and loot tracker designed for **Arc Raiders**. This tool allows streamers to track their wallet growth, raid counts, and profit-per-extraction in real-time with a clean text-based overlay for OBS.

---

## 📸 Preview
> [!TIP]
> Add a screenshot or GIF of your tracker here!
> `![App Preview]([<img width="1724" height="1920" alt="Screenshot 2026-01-22 062654" src="https://github.com/user-attachments/assets/3f56b538-6437-477d-b282-9b3819eb4270" />
])`

---

## ✨ Key Features

* **Session Gains Tracking:** Automatically calculates total profit/loss since you started your stream.
* **Dynamic Raid Counter:** Increments your raid count automatically whenever your wallet value changes.
* **Personal Best (PB):** Tracks your highest single-extraction profit during the current session.
* **OBS Integration:** Generates a clean `loot_stats.txt` file that OBS can read natively as a Text Source.
* **Privacy Focused:** No external API calls or account linking required. All data stays on your machine.

---

## 🚀 Getting Started

### 1. Prerequisites
* **Python 3.x** must be installed on your system.
* No external libraries are required (uses built-in `tkinter`).

### 2. Installation
1.  Clone this repository or download the `loot_tracker.py` file.
    ```bash
    git clone [https://github.com/](https://github.com/)[YOUR_GITHUB_USERNAME]/arc-raiders-pro-tracker.git
    ```
2.  Navigate to the directory:
    ```bash
    cd arc-raiders-pro-tracker
    ```

### 3. Usage
1.  Run the application:
    ```bash
    python loot_tracker.py
    ```
2.  **Initial Setup:** Enter your current wallet balance into the **Session Start Value**.
3.  **During Stream:** Every time you extract or finish a raid, enter your new total in **Current Wallet** and click **Log End of Raid**.

---

## 📺 How to add to OBS

1.  Open **OBS Studio**.
2.  Add a new **Text (GDI+)** Source to your Scene.
3.  Check the box **Read from file**.
4.  Browse and select the `loot_stats.txt` file located in the script's folder.
5.  (Optional) Set the font to something bold (like *Impact* or *Arial Black*) and add a text outline for better visibility.

---

## 🛠️ Project Structure

| File | Description |
| :--- | :--- |
| `loot_tracker.py` | The main GUI application and logic. |
| `loot_stats.txt` | The live output file for OBS (auto-generated). |

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Developed for the Arc Raiders Community.** *Found a bug? Open an issue or submit a Pull Request!*
