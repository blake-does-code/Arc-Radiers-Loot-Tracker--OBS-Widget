💰 Arc Raiders Pro Tracker
A lightweight, local-first loot tracker designed for Arc Raiders (or any extraction shooter) to track your daily gains, raid performance, and wallet progress in real-time on stream.

✨ Features
Real-Time OBS Integration: Automatically generates a loot_stats.txt file for a clean, text-based overlay.

Session Gains: Tracks exactly how much you've made since the start of your stream.

Raid Counter: Automatically increments your raid count every time you log a change in wallet value.

Personal Best: Keeps track of your "Best Raid" (highest single-extraction profit) during the session.

Zero Resource Impact: Uses tkinter for an ultra-lightweight footprint while you play.

🚀 How to Use
1. Requirements
Python 3.x installed on your system.

2. Setup
Download loot_tracker.py into its own folder.

Run the script:

Bash
python loot_tracker.py
Set Start Value: Enter your current wallet balance when you start your stream.

Log Raids: Every time you extract, enter your new wallet total and click LOG END OF RAID.

3. Adding to OBS
In OBS, add a new Text (GDI+) Source.

Check the box that says Read from file.

Click Browse and select the loot_stats.txt file created in the script's folder.

Style your font and colors to match your stream layout!

📂 Project Structure
loot_tracker.py: The main GUI application.

loot_stats.txt: The output file used by OBS (auto-generated).

🛠️ Configuration
You can edit the self.start_val in the code if you want to hardcode a specific starting wallet amount, or change FILE_PATH to save the output elsewhere.

🤝 Contributing
Feel free to fork this project! If you're a Python dev and want to help add a "Goal Progress Bar" or a database for long-term stats, pull requests are welcome.
