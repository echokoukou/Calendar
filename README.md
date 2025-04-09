# TGCカレンダー自動組版

## InDesignフォーマット構造
### layer
- position：玉の座標はプログラム内部で保存しない。このレイヤーの該当objectの座標（左上）が基準になる。
  - type: textFrame
  - name: R-C（行-列、1-based index）。例：3-2（3行2列目）

- tama：日付の玉（outline化済み）。S:special、P:preview、N:next
  - 今月：1〜31, S23, S24
    - ※7*5の場合：23/30(S23)、24/31(S24)の組み合わせも必要
  - 前月：P23〜P31
  - 翌月：N1〜N6

- design：固定部分全て


## エクセルファイルの処理(Python)
### 日付エクセル
### カレンダー仕様書エクセル

## 自動組版(JSX)
