# RussiaNemuro

根室海峡・北海道周辺におけるロシアトロール船の操業実態を GFW (Global Fishing Watch) AIS データから分析する。

## Structure
- `RussiaNemuro.qmd` — main analysis
- `src/` — helper R scripts
- `data/raw`, `data/processed` — local only (gitignored). Source: gakuLab shared drive (`GFW_MAIN_SHARE`)
- `output/fig`, `output/tables` — figures/tables for the paper
- `paper/` — manuscript

## ルール
- 分析範囲は必ず地図で1回出力して見せる（例：`plot01_area`）
- 図表は `plotNN_<内容>` / `tableNN_<内容>` と名付け、同じ名前で `output/fig`, `output/tables` に保存する（`save_plot()`, `save_table()`）
- チャンクラベルも同じ名前（`plot01-area`）。見出しは `## plot01 分析範囲`
- 見出し番号はQuartoの自動採番（`number-sections`）に任せ、手で振らない
