# フランチャイズ情報スクレイピングツール（Entrenet対応）

## 📘 概要
加盟店募集サイト「Entrenet」から、フランチャイズ情報を自動取得するSeleniumベースのPythonツールです。  
詳細ページまで遷移し、CSV形式で出力できるよう設計しています。

## ⚙️ 使用技術
- Python（Selenium / BeautifulSoup / pandas）
- ブラウザ制御：Chrome + WebDriver Manager
- 出力形式：CSV

## 🧭 主な処理フロー
1. 指定カテゴリ or ページ範囲をクロール  
2. JavaScript描画された詳細ページへアクセス  
3. 店舗名・初期費用・ロイヤリティ等の情報を取得  
4. pandasで整形 → CSV出力

## 📎 使用例
```bash
python scraper.py --start=1 --end=10 --output=franchise.csv
