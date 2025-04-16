# 🏏 WicketWatcher - PyDRS

**WicketWatcher** is a Python-based Third Umpire Decision Review System simulator. Built using **OpenCV**, **Tkinter**, and **PIL**, it allows users to interactively review cricket match footage, navigate frames, and simulate third umpire decisions like "Out" and "Not Out".

---

## 📽️ Features

- Frame-by-frame video navigation (fast & slow, forward & backward)
- Real-time simulation of third umpire decision-making
- Simple and interactive GUI built with Tkinter
- Decision screens: Pending, Out, and Not Out
- Smooth experience using multithreading

---

## 🧠 Architecture / Framework

The **WicketWatcher** system follows a client-server-like architecture where the **Tkinter GUI** serves as the interface, and **OpenCV** handles the backend logic for video processing and frame control. The system ensures responsiveness through the use of Python’s `threading` module for background tasks like rendering decisions.

### Key Components:
- **Tkinter GUI**: For user interaction and video display.
- **OpenCV**: For video input, frame reading, and manipulation.
- **Threading**: Ensures smooth GUI performance while simulating decisions.

---

## ⚙️ Algorithm and Process Design

The system follows a straightforward algorithm:

1. **Initialization**: Load video and setup GUI buttons and canvas.
2. **Video Playback**: Read frames and update based on navigation buttons.
3. **Frame Navigation**: Jump frames forward or backward depending on speed/direction selected.
4. **Decision Simulation**:
   - Show "PENDING" screen
   - Delay
   - Display final decision ("OUT" or "NOT OUT")
5. **Rendering**: Continuously update and redraw the current frame on the canvas.
6. **Exit Condition**: Stop playback when end of video is reached.

---

## 🛠️ Technologies Used

- Python 3.x
- OpenCV
- Tkinter
- Pillow (PIL)
- Imutils

---

## 🚀 Getting Started

### Prerequisites

Install the required packages using pip:

### Clone the Repository

```bash
git clone https://github.com/yourusername/WicketWatcher.git
cd WicketWatcher
```

### Run the Application

Ensure the following files are present in your project folder:
- `clip.mp4` – Sample cricket video clip
- `WELCOME.jpg` – Initial welcome screen
- `PENDING.jpg` – Third umpire "Decision Pending" image
- `OUT.jpg` – Out decision image
- `NOT_OUT.jpg` – Not Out decision image

Then run:

```bash
python main.py
```

---

## 📁 Folder Structure

```
WicketWatcher/
├── clip.mp4
├── WELCOME.jpg
├── PENDING.jpg
├── OUT.jpg
├── NOT_OUT.jpg
├── main.py
└── README.md
```

---

## 🎮 Controls

| Button               | Action                         |
|----------------------|--------------------------------|
| << Previous (fast)   | Go back 25 frames              |
| << Previous (slow)   | Go back 2 frames               |
| Next (slow) >>       | Go forward 2 frames            |
| Next (fast) >>       | Go forward 25 frames           |
| Give Out             | Show "Out" decision            |
| Give Not Out         | Show "Not Out" decision        |

---

## 📷 Screenshots
> ![0](https://github.com/user-attachments/assets/3fd8e852-8e2e-4586-8783-d6e67b569528)
> ![1](https://github.com/user-attachments/assets/5e4c2cb0-4734-4486-aaf9-03806ba9f8d8)
> ![2](https://github.com/user-attachments/assets/ef3032db-20fe-45ef-928f-4021500dd7f5)
> ![4](https://github.com/user-attachments/assets/7118d146-4493-4697-b6bc-51f1f898747f)

---

## 🤝 Contributing

Want to make it better? Fork the repo, make changes, and open a pull request!

---

## 📄 License

This project is for educational and demonstration purposes only.

---
