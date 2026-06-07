# 更新ガイド

## News を追加する

[`_data/news.yml`](_data/news.yml) の **先頭** に追加する。

```yaml
- type: acceptance        # acceptance（緑）または reward（赤）
  title: "論文タイトル"
  link: "https://arxiv.org/abs/xxxx"  # なければ "" のまま
  description: "got accepted to **VENUE 2026**."
```

---

## 論文を追加する

[`_data/publications.yml`](_data/publications.yml) の **先頭** に追加する。

```yaml
- title: "論文タイトル"
  category: conferences   # conferences / journals / domestic
  venue: "VENUE 2026"
  authors: "<strong>Shumpei Takezaki</strong>, 著者2, 著者3"
  paperurl: "https://arxiv.org/abs/xxxx"  # なければ削除してOK
  code: "https://github.com/..."          # なければ削除してOK
  date: "2026-01-01"
```

**category の使い分け：**
| 値 | 表示セクション |
|---|---|
| `conferences` | Conference Papers |
| `journals` | Journal Articles |
| `domestic` | Domestic Conference / Presentation in Japan |

---

## 受賞・グラントを追加する

[`_data/others.yml`](_data/others.yml) の該当セクションの **先頭** に追加する。

```yaml
awards:
  - text: "新しい受賞の説明, 2026."   # ← ここに追加
  - text: "既存の受賞..."

grants:
  - text: "新しいグラント..."          # ← ここに追加
  - text: "既存のグラント..."
```

---

## ローカルでプレビューする

```bash
bundle exec jekyll serve
# → http://localhost:4000 で確認
```
