# 🔒 Encrypted Diary (Python CLI)

A secure, text-based diary application—your personal thoughts, encrypted and protected with a password using strong cryptography. Write, view, and read diary entries in privacy and ease!

---

## ✨ Features

- **Password authentication:** Only you can open your diary
- **All entries are encrypted with Fernet (symmetric encryption)**
- **Create new entries** (title + content), timestamped and saved securely
- **View all entries:** See a numbered list of your entries with filenames
- **Read any entry:** Decrypt and display contents for any saved diary entry
- **Data is kept in local `entries/` directory** as encrypted files, never in plain text
- **Easy command-line prompts** and clear feedback
- **Cross-platform, no internet needed**

---

## 🚀 How to Run

1. **Python 3 required**
2. **Install the required package:**
    ```
    pip install cryptography
    ```
3. **Save code as `diary.py`**
4. **Run in terminal/cmd:**
    ```
    python diary.py
    ```

---

## 🧑‍💻 Usage

- **Set your password in the code** (look for the variable `correct_password = "PassW0rd"`—change this!)
- **When prompted, enter your password to proceed**
- **Menu options:**
  1. Create a New Entry
  2. View All Entries
  3. Read an Entry
  4. Exit

---

## 🗂️ How It Works

- On first run, generates a Fernet key file (`secret.key`)
- Diary entries are encrypted before saving; content is never stored in plain text
- You can view all entry filenames (with timestamps) or select for reading
- All data is stored locally; only you can read or add to your diary

---

## ❗ Security Note

- The password is hardcoded for demo; for *real* secrets, use a hashed/hidden password prompt or environment variable!
- Don’t lose `secret.key`—you won’t be able to decrypt your entries

---

## 📄 License

MIT License — free for learning, teaching, and tinkering.

---

A perfect project for Python learners who want to combine cryptography, file handling, and CLI design!
