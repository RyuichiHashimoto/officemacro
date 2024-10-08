# README_for_user.md

- [1. 本資料対象者](#1-本資料対象者)
- [2. 本資料の内容](#2-本資料の内容)
- [3. 使用方法](#3-使用方法)
  - [3.1. パワーポイントアドインを作成する。](#31-パワーポイントアドインを作成する)
  - [3.2. パワーポイントでマクロを読み込む。](#32-パワーポイントでマクロを読み込む)
  - [3.3. リボンに編集タブが追](#33-リボンに編集タブが追)
- [4. マクロ一覧](#4-マクロ一覧)
  - [4.1. arrowOneToN](#41-arrowoneton)
  - [4.2. arrowSerial](#42-arrowserial)
  - [4.3. copypos](#43-copypos)
  - [4.4. setpos\_tate](#44-setpos_tate)
  - [4.5. setpos\_yoko](#45-setpos_yoko)
  - [4.6. reduce\_width](#46-reduce_width)
  - [4.7. reduce\_height](#47-reduce_height)



## 1. 本資料対象者
パワーポイントマクロを使用したい人

## 2. 本資料の内容
パワーポイントマクロの使用手順および利用可能なマクロ一覧を示す。

## 3. 使用方法
### 3.1. パワーポイントアドインを作成する。
1. macro.pptmをパワーポイントで開く。
2. macro.pptmの操作画面のファイルタブをクリックする。
3. 「名前を付けて保存」からppam（パワーポイントアドイン）として保存する。

### 3.2. パワーポイントでマクロを読み込む。
1. パワーポイントファイルを新規作成する。
2. 開発タブからアドイングループのPowerPointアドインを選択する。
3. 新規追加ボタンをクリックして、3.1で作成したパワーポイントマクロを選択する。
4. 選択可能なアドイン一覧に選択したパワーポイントマクロが表示されるので、それを読み込む。

### 3.3. リボンに編集タブが追
1. 3.2終了後、開いているパワーポイントウィンドウを一度全て×ボタンで消す。
2. 再度任意のパワーポイントファイルを開く。
   

## 4. マクロ一覧
### 4.1. arrowOneToN
- 使用目的
    - このマクロは、最初に選択した図形から、2番目以降に選択したすべての図形に対して直線の矢印コネクタを作成する。
    - 複数の図形に対して、一つの図形から矢印を引きたい場合に使用する。

- 使用手順
  1. PowerPointのスライド上で、矢印の元になる図形を最初に選択する。
  2. その後に矢印をつなげたい他の図形を追加選択する。
  3. マクロを実行する。
     - これにより、最初に選択した図形から2番目以降の各図形に向けて、直線の矢印コネクタが作成される。
     - なお、図形が2つ以上選択されていない場合、メッセージボックスが表示され、マクロは終了される。

### 4.2. arrowSerial
- 使用目的
  - このマクロは、選択した図形の順番に従って、それぞれの図形を直線の矢印コネクタで接続する。
  - 複数の図形に対して、選択した順に図形を矢印でつなげる。

- 使用手順:
  1. PowerPointのスライド上で、矢印でつなげたい図形を順番に選択する。
  2. マクロを実行する。
     - これにより、選択した順番に従って、それぞれの図形間に直線の矢印コネクタが作成される。
     - なお、図形が2つ以上選択されていない場合、メッセージボックスが表示され、マクロは終了する。

### 4.3. copypos
- 使用目的
  - このマクロは、選択した図形の位置（上端、左端）とサイズ（幅、高さ）をコピーして保存する。

- 使用手順
    1. PowerPointのスライド上で、図形を選択する。
    2. マクロを実行する。
       - これにより、選択した図形の位置情報とサイズが保存される。

### 4.4. setpos_tate
- 使用目的
  - このマクロは、copyposで保存した位置情報とサイズを選択した図形に適用する。
  - なお、貼り付け先の図形の縦横比が固定の場合、高さがそろうようにサイズ情報が貼り付けされる。

- 使用手順:
  1. copyposマクロを実行して、サイズと位置情報をコピーしておきます。
  2. 適用したい図形を選択します。
  3. setpos_tateマクロを実行する。
     - これにより、1でコピーしたサイズと位置情報が選択した図形に適用されます。

### 4.5. setpos_yoko
- 使用目的
  - このマクロは、copyposで保存した位置情報とサイズを選択した図形に適用する。
  - なお、貼り付け先の図形の縦横比が固定の場合、横幅がそろうようにサイズ情報が貼り付けされる。

- 使用手順:
  1. copyposマクロを実行して、サイズと位置情報をコピーする。
  2. 適用したい図形を選択する。
  3. setpos_tateマクロを実行する。
     - これにより、1でコピーしたサイズと位置情報が選択した図形に適用されます。
  
### 4.6. reduce_width
- 使用目的
  - このマクロは、選択された図形の幅を特定の単位（0.2cm）に基づいて縮小するために使用します。
  - 選択された図形の幅を0.2cm単位で最も近い値に減少される。

- 使用手順:
  1. PowerPointのスライド上で、幅を減少させたい図形を1つ以上選択する。
  2. マクロを実行する。
     - これにより、選択されたすべての図形の幅が0.2cm単位で最も近い値に減少される。
     - なお、図形が選択されていない場合、メッセージボックスが表示され、マクロは終了する。
  
### 4.7. reduce_height
- 使用目的
  - このマクロは、選択された図形の高さを特定の単位（0.2cm）に基づいて縮小するために使用する。
  - 選択された図形の高さを0.2cm単位で最も近い値に減少される。

- 使用手順
  1. PowerPointのスライド上で、高さを減少させたい図形を1つ以上選択する。
  2. マクロを実行する。
     - これにより、選択されたすべての図形の高さが0.2cm単位で最も近い値に減少される。
     - なお、図形が選択されていない場合、メッセージボックスが表示され、マクロは終了する。

