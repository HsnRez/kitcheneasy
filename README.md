# キッチン在庫 / Kitchen Stock

A small, self-contained kitchen stock-take app for foods, drinks and other kitchen
supplies. Default language is **日本語**, with **繁中 / English** switchable at the top —
your choice is remembered.

Everything (items, categories, photos) is stored **locally in your browser**
(IndexedDB). No account, no server, no build step — just one HTML file.

## Features

- **Categories** (食品 / 調味料 / 飲み物 …) — add, rename and delete your own from the app
  (tap **⚙ カテゴリ編集**). Filter the list by category with the chips at the top.
- **Front page** lists items **most-urgent first** — items marked *empty* / *to buy* and
  those with the lowest quantity float to the top.
- **Search** by name or memo.
- **Item page** (tap any item):
  - **Photo** — take one with the camera or pick from the gallery (auto-resized).
  - **Quantity** with quick − / ＋ steppers and a free unit (本・個・g …).
  - **State** — 空 / 要購入 / 半分 / 開封済 / 新品 (empty / to buy / half / opened / full-new).
  - **Memo** field at the bottom for notes.
- **Add** with the ＋ button, bottom-right.

## Usage

Open `index.html` in any modern browser (works great on a phone — "Add to Home Screen"
for an app-like feel). Data lives in that browser profile.

## Development

No dependencies and no build step — a single `index.html` with inline CSS and JS.
Data model: two IndexedDB stores, `items` and `depts`.
