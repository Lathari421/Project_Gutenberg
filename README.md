# Project Gutenberg 中文書籍爬蟲專案

本專案使用 Python 自動化爬取 Project Gutenberg 網站上的中文書籍，共成功下載 **403 本書籍**，每本包含書名、作者與完整內文，並儲存為文字檔（`.txt` 格式）。

---

## 📦 安裝套件

請先安裝以下 Python 套件（版本可透過 `pip list` 或 `conda list` 查看）：

**Python version**: 3.11.11

- `requests==2.32.3`
- `beautifulsoup4==4.12.3`
- `lxml==5.3.2`

安裝指令如下：

```bash
pip install requests beautifulsoup4 lxml
```

## 🧰 使用套件（於程式中引用）
```python
from bs4 import BeautifulSoup as bs
import requests as req
from pprint import pprint
import re  # 正規表達式模組
import os, json
from time import sleep
```
## ▶️ 如何執行程式
若使用 Jupyter Notebook（.ipynb）
打開 project_gutenberg/project_gutenberg.ipynb，依序執行每個 Cell。

若使用 Python 檔案（.py）
請開啟終端機，進入專案資料夾後執行：

```bash
python project_gutenberg/project_gutenberg.py
```

## 📈 成果展示

1.總書本download截圖: project_gutenberg.png （位於專案資料夾中）

2.影片連結: https://drive.google.com/file/d/1oKKxH0kiQuwFC-P8GJ3hqj8fEPPQl1Ze/view?usp=sharing
