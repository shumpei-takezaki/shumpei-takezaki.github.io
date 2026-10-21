# 更新ガイド

## News を追加する

[`_data/news.yml`](_data/news.yml) の **先頭** に追加する。

```yaml
- date: "2026-08"
  text: "A paper was accepted to **IEEE Access**."
```

- `date` は `"YYYY-MM"` の形式。画面の左列に表示される。
- `text` は 1 文で短く書く。論文タイトルは書かない（論文は Publications に載る）。
- 会議名・ジャーナル名・賞の名前は `**…**` で太字にする。
- 書き方の例：

| 内容 | text |
|---|---|
| 1 本採択 | `A paper was accepted to **IJCNN 2026**.` |
| 複数本採択 | `Two papers were accepted to **IJCNN 2026**.` |
| 受賞 | `Received the **Best Paper Award** at **ICDAR 2025 Workshop**.` |

- News は新しい 5 件だけが最初に表示され、残りは **Show more** を押すと開く。
  表示件数を変えるときは [`_pages/about.md`](_pages/about.md) の `news_visible` を編集する。

---

## 論文を追加する

[`_data/publications.yml`](_data/publications.yml) の **先頭** に追加する。

```yaml
- title: "論文タイトル"
  category: journals      # conferences / journals / domestic
  venue: "IEEE Access"
  authors: "<strong>Shumpei Takezaki</strong>, 著者2, 著者3"
  paperurl: "https://ieeexplore.ieee.org/..."  # なければ削除してOK
  code: "https://github.com/..."               # なければ削除してOK
  date: "2026-08-04"
```

- `date` は並び順に使うだけで、画面には出ない。会議なら開催日、ジャーナルなら公開日を入れる。
- 自分の名前は `<strong>…</strong>` で太字にする。
- 日付・著者のフルネーム・URL は Google Scholar の論文ページ（タイトルをクリック）で確認できる。

**category の使い分け：**

| 値 | 表示セクション |
|---|---|
| `conferences` | Conference Papers |
| `journals` | Journal Articles |
| `domestic` | Domestic Conference / Presentation in Japan |

**venue の書き方：**

- `conferences` / `journals` では、venue が青緑色のバッジになる。
- `(` より前がバッジ、括弧の中は色なしの文字になる。
  - `"ISBI 2026 (Best Paper Award-Runner Up)"` → バッジ「ISBI 2026」＋ (Best Paper Award-Runner Up)
- ジャーナル名には年を付けない（例：`"IEEE Access"`）。会議名には年を付ける（例：`"WACV 2025 (Oral)"`）。
- `domestic` はバッジにならず、斜体の文字で表示される。

---

## 受賞・グラント・ワークショップ運営を追加する

[`_data/others.yml`](_data/others.yml) の該当セクションの **先頭** に追加する。

```yaml
awards:
  - text: "新しい受賞の説明, 2026."   # ← ここに追加
  - text: "既存の受賞..."

grants:
  - text: "新しいグラント..."          # ← ここに追加
  - text: "既存のグラント..."

workshops:
  - text: "[ワークショップ名](URL), ACCV 2026 Workshop, December 15, 2026, Osaka, Japan. Organizer."  # ← ここに追加
```

- `text` は Markdown が使える。ワークショップ名は `[名前](URL)` でリンクにする。
- Others ページの「Workshop Organization」に表示される。

---

## ローカルでプレビューする

```bash
bundle exec jekyll serve --config _config.yml,_config_docker.yml
# → http://localhost:4000 で確認
```

`--config _config.yml,_config_docker.yml` が必要。付けないと CSS / JS が公開サイトのものを読み込み、
SCSS や JS の変更（ダークモードなど）がローカルに反映されない。
`_config.yml` を変更したときだけ、サーバーを再起動する。

---

## ライト / ダークモード

- ヘッダー右端のアイコン（太陽 / 月）で切り替える。
- 初めて開いたときは OS の設定に合わせ、切り替えるとブラウザに記憶される。
- 色の定義は [`_sass/theme/_toggle.scss`](_sass/theme/_toggle.scss)。
  ページ内の CSS に色を書くときは、固定の色ではなく `var(--line-color)` などの変数を使う。
