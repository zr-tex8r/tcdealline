tcdeadline パッケージ
=====================

LaTeX: \today を(締切まで)“あと○日”にするやつ

### 前提環境

  * フォーマット： LaTeX
  * エンジン： pTeX / upTeX
  * DVIウェア： なんでも
  * 依存パッケージ/ソフトウェア： なし

### インストール

  - `*.sty` → $TEXMF/tex/platex/tcdeadline

※単に TeX ファイルを同じディレクトリに置くのでもOK。

### 使い方

パッケージを読み込む。
すると、`\today` の出力が「あと○日○時間」に変更される。

    \usepackage[<締切日時>]{tcdeadline}

締切日時は `年/月/日@時:分` の形式で指定する。

例：

    \documentclass[dvipdfmx]{orzthesis}
    \usepackage[2014/01/31@15:00]{tcdeadline}%←これを追加!
    \進捗どうですか
    \title{卒論はNP困難}
    \usepackage{graphicx,color}
    %(以下略)

--------------------
Takayuki YATO (aka. "ZR") 
http://zrbabbler.sp.land.to/
