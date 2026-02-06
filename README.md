# 👻 Ghost-OS: Ephemeral Virtual Environment

**Ghost-OS** is a browser-based, RAM-only virtual machine. It transforms this static GitHub Pages site into a functional x86 computing environment using WebAssembly.

---

## 🛡️ Privacy & Liability Shield (PLEASE READ)

Ghost-OS is designed for high-privacy, ephemeral computing. By using this tool, you acknowledge and agree to the following:

### 1. No Data Persistence
* **Execution Environment:** All OS operations occur strictly within your browser's RAM (volatile memory). 
* **Zero-Server Footprint:** No data is ever uploaded, stored, or transmitted to GitHub, the creators, or any third-party servers.
* **Wipe-on-Close:** Once the browser tab is refreshed or closed, the entire virtual environment and all unsaved data vanish instantly. For best performance open in private browser.

### 2. Local Logging (User-Controlled)
* The "Save Session Log" feature is a **client-side-only** process. 
* When clicked, the terminal output is packaged into a local memory buffer (Blob) and downloaded directly to your physical machine. 
* This data never leaves your computer; you are the sole custodian of any logs you choose to generate.

### 3. Disclaimer of Liability
* **AS IS Basis:** This software is provided "as is" without any warranty or security guarantees.
* **No Responsibility:** The creators of Ghost-OS shall not be held liable for:
    * Loss of data due to tab crashes or accidental refreshes.
    * Exposure of sensitive data analyzed within the VM.
    * Any damages resulting from the use or inability to use this tool.
* **User Security:** While the environment is sandboxed in the browser, the security of the host machine and the physical environment remains the user's responsibility.

---

## 🚀 How to Use

1.  **Boot:** Click the "I ACCEPT" button on the splash screen to initialize the WebAssembly engine.
2.  **Analyze:** Drop in your code or logs (within the limits of the minimal Linux environment).
3.  **Save:** Use the "SAVE SESSION LOG" button in the status bar to download a text record of your work to your local machine.
4.  **Destroy:** Click "WIPE RAM / SHUTDOWN" or simply close the tab to delete the session forever.

---

## ⚠️ Technical Limitations
To maintain the "Ghost" (ephemeral) nature of this OS, the following limitations exist:
Networking: Due to browser security (CORS/Socket policies), the VM does not have direct access to the raw internet. You cannot ping or ssh out to external servers.
Performance: The CPU is emulated via WebAssembly. It is roughly 10x-20x slower than your host machine. It is designed for scripts and text processing, not heavy computation.
Storage Size: You are limited by your browser's allocated memory (currently set to 32MB). Large files may cause the VM to crash or "Out of Memory" errors.
Clipboard: Some browsers require a manual "Paste" via a right-click or specific menu if the OS doesn't automatically capture your keyboard's Ctrl+V.

---

## ⚖️ License
This project is released under the **MIT License**. See the `LICENSE` file for full details.
