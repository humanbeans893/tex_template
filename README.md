# LaTeX Template for Seminar Reports

研究室ゼミ用のLaTeX論文テンプレートです。

## 概要

このテンプレートは、研究報告やゼミ資料の作成に最適化されています。以下の機能を含みます：

- 日本語対応（`jresume.cls`使用）
- 数式、図表、参考文献の記述例
- 状態空間モデルなどの数式サンプル
- コメント・添削機能（色付きテキスト）

## ファイル構成

```
.
├── main.tex         # メインのTeXファイル
├── jresume.cls      # 日本語レジュメ用クラスファイル
├── reference.bib    # 参考文献データベース
├── latexmkrc        # latexmk設定ファイル
└── figures/         # 図を格納するフォルダ
```

## 使い方

### コンパイル

```bash
latexmk main.tex
```

または

```bash
platex main.tex
pbibtex main
platex main.tex
platex main.tex
dvipdfmx main.dvi
```

### テンプレートの編集

1. `main.tex`を開く
2. 青字（`\guide{}`）の指示に従って各項目を記入
3. 記入後は青字部分を削除

## 主な機能

### コメント・添削用コマンド

```latex
\mizushima{赤字でコメント}
\mizushimaerase{取り消し線付きテキスト}
```

### カスタムコマンド

```latex
\argmax  % arg max
\argmin  % arg min
```

## 必要なパッケージ

- graphicx
- amsmath, amssymb
- natbib
- hyperref
- その他（main.texのプリアンブル参照）

## ライセンス

研究室内での使用を想定しています。
