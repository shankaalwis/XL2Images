# 📥 Excel Image Downloader

A simple Python script that reads image URLs from an Excel file and downloads them to a local folder. Ideal for bulk downloading product images, datasets, or reference assets.

---

## 🚀 Features

- ✅ Reads `.xlsx` files using `openpyxl`
- ✅ Downloads images via `requests`
- ✅ Supports custom columns and row ranges
- ✅ Skips invalid or missing URLs
- ✅ Automatically names files from URL or assigns a fallback name

---

## 📂 How It Works

1. Place your Excel file (e.g. `images.xlsx`) in the project directory.
2. The script reads URLs from a specified column (default: `A`).
3. It downloads and saves each image to the `downloaded_images` folder.

---

## 📄 Example Excel Layout

| A (Image URL)                     |
|----------------------------------|
| https://example.com/image1.jpg   |
| https://example.com/image2.jpg   |

> You can change the column or row starting point in the script.

---

## 🛠 Configuration

Open the script and edit the following lines as needed:

```python
EXCEL_FILE = "products_list.xlsx"
COLUMN_WITH_URLS = 'A'
START_ROW = 2
DOWNLOAD_DIR = "downloaded_images"
````

---

## ⚙️ Installation

1. **Clone the repo:**

```bash
git clone https://github.com/your-username/excel-image-downloader.git
cd excel-image-downloader
```

2. **Install dependencies:**

```bash
pip install -r requirements.txt
```

> Or manually install:
> `pip install openpyxl requests`

3. **Run the script:**

```bash
python image_download_script.py
```

---

## 🧯 Error Handling

* Invalid URLs are skipped with a warning.
* Files are named automatically based on the URL path.
* You can add retry logic or logging for advanced use.

---

## 📄 License

MIT License. Free to use, modify, and distribute.

---

## 🙌 Contributions

Feel free to fork and submit pull requests for improvements or feature additions.

```

---

Let me know if you'd like to generate a `requirements.txt` file or want this in a zip folder format!
```
