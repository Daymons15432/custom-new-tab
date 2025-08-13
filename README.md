# Custom New Tab

**Custom New Tab** is a Chrome extension that lets you replace the default `chrome://newtab` page with your own custom design.

---

## ✨ Features

- **Customizable Design** – Easily change the layout, colors, and animations.
- **Easy Icon Replacement** – Change the favicon directly from `manifest.json`.

---

## 📂 Project Structure

```
.
├── manifest.json        # Extension configuration
├── newtab.html          # HTML structure and styles for the New Tab page
├── icon256.png          # Example icon (replaceable)
```

---

## ⚙️ Installation

### **1. Install as Local Extension**
1. **Download or clone** this repository to your local machine.
2. Extract the ZIP file if it is compressed.
3. Open **Google Chrome** (or other Chromium-based browsers like Edge, Brave).
4. Navigate to:
   ```
   chrome://extensions/
   ```
5. Enable **Developer Mode** (top right corner).
6. Click **Load unpacked**.
7. Select the folder containing the extension files (`manifest.json` should be in this folder).
8. Open a new tab to see your custom page.

---

## 🖼️ Customization

### **1. Change the favicon**
- Open `manifest.json`.
- In the `"icons"` section, replace the file name with your desired icon file.
- For example:
  ```json
  "icons": {
    "256": "myicon256.png"
  }
  ```
- Make sure the number matches the icon size (e.g., `256` for `256x256`).

### **2. Edit the page design**
- Modify `newtab.html` to adjust colors, layout, and animations.
- All CSS is embedded inside the `<style>` tag or you can create a file to separate them.
- For adding scripts:
  - Create a separate `.js` file (e.g., `script.js`).
  - Link it inside `newtab.html`:
    ```html
    <script src="script.js"></script>
    ```

---

## 🛠️ Development Notes

- This extension overrides Chrome’s default New Tab page.
- Only works in Chromium-based browsers (Chrome, Edge, Brave, etc.).
- If your changes are not showing, try disabling and reloading the extension.

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

---

**Created by [Hakiou Derion](https://github.com/Daymons15432)**
