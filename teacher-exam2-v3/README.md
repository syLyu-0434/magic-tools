# 教師檢定考刷題 v3

這一版把題庫從 `teacher-exam.html` 拆到 `data/teacher-exam/`。

## 檔案結構

```text
teacher-exam.html
data/teacher-exam/ideology/110.json
data/teacher-exam/ideology/111.json
data/teacher-exam/ideology/112.json
data/teacher-exam/ideology/113.json
data/teacher-exam/ideology/114.json
data/teacher-exam/development/110.json
data/teacher-exam/development/111.json
data/teacher-exam/development/112.json
data/teacher-exam/development/113.json
data/teacher-exam/development/114.json
data/teacher-exam/curriculum/110.json
data/teacher-exam/curriculum/111.json
data/teacher-exam/curriculum/112.json
data/teacher-exam/curriculum/113.json
data/teacher-exam/curriculum/114.json
```

## 更新年度題庫

之後新增 115 年，只要新增對應 JSON，並在 `teacher-exam.html` 的 `SUBJECT_PATHS` 補路徑即可。

## 注意

因為本頁使用 `fetch()` 載入 JSON，直接雙擊本機 HTML 可能會被瀏覽器擋下。請放在 GitHub Pages，或用本機伺服器測試。
例如：

```bash
python3 -m http.server 8000
```

再開啟 `http://localhost:8000/teacher-exam.html`。
