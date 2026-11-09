**Made by someone** this tool has been set private cause it will the ruin the game for everyone

A lightweight, external auto-reverse tool I built for **Gota.io** (and other Agar-style games). Instead of messing with browser memory, extensions, or WebSocket hooks, it reads screen pixels around your target cell in real time and hits your split/reverse key the instant the enemy cell shrinks or splits.



https://github.com/user-attachments/assets/6d06d10c-836e-4556-9d48-f652d7fac65d


---

## How It Works

When you lock onto a cell, a small black crosshair glides out to the cell and follows its movement smoothly.

- If the player is just moving around normally, the crosshair drifts along with it..
- The moment they press split (or shrink suddenly), their cell border pulls back across the crosshair and the tool instantly fires your reverse/split key.
- Every trigger is strictly **single-shot**—once it fires, it disarms itself automatically so it won't spam your keys.

- 
<img width="1380" height="891" alt="Screenshot 2026-11-06 171835" src="https://github.com/user-attachments/assets/713be272-9d53-4990-b85d-af2d4dad69ce" />
---

## Modes

- **Fixed Mode (Toggle — default `X`)**  
  Aim anywhere inside an enemy cell and press your toggle key. The crosshair glides out, tracks the cell's border, and fires as soon as the cell splits.

- **Smart Mode (Toggle — default `Z` / `M`)**  
  Locks onto the exact RGB color under your cursor and tracks the cell's border. As soon as that color changes past your sensitivity threshold, it fires. Great when playing with custom background colors or themes.

- **Movable Mode (Hold — default `C` / `P`)**  
  Hold the key down to sample directly under your live mouse cursor without locking the crosshair in place.
  
<img width="282" height="69" alt="Screenshot 2026-11-06 172547" src="https://github.com/user-attachments/assets/70c1286f-3ec0-4776-954d-0ebcc8951469" />

---

## Main Features

- **Directional Tracking**: You don't have to pixel-hunt the very edge of a cell—aim inside the cell and the crosshair automatically glides out .
- **Controlled Glide Speed**: Crosshair movement is tuned so it follows normal drift smoothly without outrunning a cell when it shrinks or splits.
- **Auto-Aim Snap & Cursor Tether**: Can automatically snap your cursor to the target right before firing your split, or tether your mouse directly to the tracking crosshair.
- **Click-Through Black Crosshair**: Clean overlay reticle that stays on top of the game without stealing focus or blocking mouse clicks.
- **under 1 ms detection and fire time**

<img width="211" height="86" alt="image" src="https://github.com/user-attachments/assets/ee861a3c-b24a-41d3-bc21-90a511e910ff" />


---

## Best In-Game Settings (Gota.io)

For the cleanest tracking in all Modes:
1. Use a **Dark / Black background**.
2. Turn off **Skins** so cells are solid colors.
3. lower animation delay.
4. be smart and play anonymously.

---

## Setup & Running **you dont need this cause the tool is private**

Make sure you have Python 3.10+ installed along with `customtkinter` and `Pillow`:

```bash
pip install customtkinter pillow
```

Then either double-click **`run.bat`** or run:

```bash
python main.py
```

Set your hotkeys and sensitivity in the menu, click **Apply & Save Settings**, and you're good to go.
