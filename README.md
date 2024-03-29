# ロボットラーニング研究室の修論テンプレート
## 概要
ロボットラーニング研究室に特化したテンプレートです．\
[Overleaf](https://ja.overleaf.com/)上で使うことを想定して作られていますが，ローカルでもコンパイルできます．

ロボットラーニング研究室で修論を執筆する際に守る必要のある事柄がPDFに記載されています．\
**当研究室で修論を書く人はこれを使ってください**．

## ファイル構成
```
.
├── figures/                図のファイルを入れます．(サンプルファイル在中)
├── tex_files/              TeXファイルを入れます．(既に推奨構成のファイルが生成されています)
│   ├── 00_abstract.tex
│   ├── 10_introduction.tex
│   │   
│   └── 90_appendix.tex
├── info.tex                修論情報を記載するファイル (後述)
├── jIEEEtran.bst           BibTeXのスタイルファイル (https://ctan.org/pkg/jieeetran)         
├── latexmkrc               Overleaf内部処理用 (いじる必要なし)     
├── mthesis.tex             TeXのマスターファイル
├── naist-rll-jmthesis.sty  NAIST有志作成のスタイルファイルを研究室向けに改造
├── pdf_verX.X.pdf          公開バージョンに対応したPDF
├── README.md               
└── reference.bib           BibTeX用のファイル
```
- tex_files/内でファイルが章の順番通りに並ぶよう，ファイル名の先頭に数字を入れています (e.g., 00_abstract.tex)．
- 章などを増やしたい時は，65_real_experiment_result.texのように適切な番号を頭に付与してください．

## 使い方
1. ダウンロードしたZipファイルを[Overleaf](https://ja.overleaf.com/)にアップロード
2. プロジェクト名を変更 (以下の〇〇は名前)
   - 例: ロボットラーニング研究室の修論テンプレート -> 修士論文_〇〇_2023
3. 左上の**メニュー**をクリック
   - ~~コンパイラを**LaTeX**に変更~~ (コンパイラでpdflatexが選択されていることを確認)
   - (任意) スペルチェックを**オフ**に (日本語対応していないため)
4. **リコンパイル**を押してコンパイルが通りPDFが生成されることを確認
5. info.texに記載されている内容をファイル内の指示に従って編集すること

## 更新履歴
- 2023.12.18 - Ver 1.1 / M2向けに公開
- 2023.12.21 - Ver 1.2 / 副査が4人以上いる場合に対応
- 2024.01.10 - Ver 1.3 / 図題と表題を英語に，PDFの見出しの文字化けを防ぐ
- 2024.01.11 - Ver 1.5 / bibtexスタイルをjIEEEtranに変更，スタイルファイルを統合
- 2024.01.14 - Ver 1.6 / 1.3にアプローチを追加．コンパイラ設定がpdflatex (デフォルト)のまま使えるように修正

## Todoリスト
- 英語版準備

___
謝辞: 田原君のコードを一部参考にしています．ここに謝意を示します．
