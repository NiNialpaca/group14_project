# Wordle: Multi‑Player / Single-Player Edtion

> **Group 14 • Python • Pygame • 2025**

This project is a local party / single version of the classic *Wordle* game. Up to **6 players** take turns guessing the **same hidden five‑letter word**, compete for points, and enjoy a lively scoreboard—all wrapped in a colorful GUI built with **Pygame**.

---

## 🛠 Prerequisites
| Tool | Version | Notes |
|------|---------|-------|
| Python | 3.10 or newer | Other versions may work but are untested |
| pip packages | `pygame`, `pyenchant`, `subprocess` | 


All other files (images, `word.py`, etc.) are already included in this repository / zip.

---

---
## 🖥️ How to Run
```bash
git clone https://github.com/weiouo-0817/oop-2025-proj-wordle.git
```
```bash
cd oop-2025-proj-wordle
```
```bash
sudo apt install python3.10-venv   # (optional) create and activate a virtual‑env
```
```bash
python -m venv venv                # (optional) create and activate a virtual‑env
```
```bash
source venv/bin/activate           # Windows: .\venv\Scripts\activate
```
```bash
pip install pygame pyenchant
```
```bash 
python main.py        
```
> **Note:**  If `pyenchant` complains about dictionaries, install system packages:<br>`sudo apt install libenchant-2-2` (Ubuntu) or brew equivalent.

---

## 📁 Project Structure
```
oop-2025-proj-wordle/
├── main.py           # game entry‑point (this script launches everything)
├── word.py           # list of valid 5‑letter words
├── multiwordle.py
├── singlewordle.py
├── image/
│   ├── 23671474_m.jpg    # title / menu background
│   └── 123.jpg           # in‑game background
│   └── 8623_m.JPG           
└── README.md         # ← you are here
```

---
## 🎮 Game Flow - Multi‑Player
1. **Select player count** (1–6) on the menu.
2. **Enter player names** – highlighted row shows whose name you are typing.
3. **Guess turns** – each player types a 5‑letter word ⏎.   
                   – each player can guess 3 times per word   
                   – will go 5 round
4. **Color feedback** follows Wordle rules:
   * 🟩 **Green** – correct letter & position (+3 pts)  
   * 🟨 **Yellow** – letter exists but wrong spot (+2 pts)  
   * ⬛ **Gray** – letter not in word (0 pts)
5. **Scoreboard** updates instantly. First to solve scores a bonus!
6. Press **Home** to restart or **End Game** to see the final ranking.

---

## 📝 Scoring Summary

| Tile colour | Points |
|-------------|--------|
| Green 🟩 | **+3** |
| Yellow 🟨 | **+2** |
| Gray ⬜/⬛ | 0 |

----

## 👥 Credits
 **chen-wei wu** /     Hope you have fun to play the game !
