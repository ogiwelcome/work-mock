date: 2022/02/08

status: doing

member: 荻野真浩

(ここら辺はassignerに入れてもいい)

# documentにgitを導入するDR

## 経緯
- 従来までのdocument管理方法ではあらゆる資料が dropbox や openproject 、google spread-sheet などに散乱しており、新人で入ってきた自分にはわかりにくいと感じた。
- ある程度中央に集中させ、「ここを見ればいい」といった感じの管理をするにはgit管理が優れていると感じるので、これについて議論し、決定まで行う(議論のみで判断主体が他者に回る場合はそのままこれを見せればいい)
- 今議論に上がっているのが二つなので他に候補があれば適宜追加する

## 比較
(ここら辺の項目はある程度自由に)

|| 従来の管理(spread sheet+dropboxとか) | Git管理 |
|----|----|----|
|管理しやすさ| ⭕️ | ⭕️(*1) |
|参考しやすさ| ❌ | ⭕️ |
|version比較| ❌ | ⭕️ |
|書きやすさ| ⭕️ | 🔺 |

*1：git操作ができない人だと困る

## メリット・デメリット
- 従来の管理
    - メリット
        - 何より簡単に作れる
        - 命名でパッとわかる
    - デメリット
        - version管理がしにくい(導入時のエラー対応などの追記がしづらい)
        - 一括的な管理でなく散漫としている
- git管理
    - メリット
        - directoryのような階層的管理ができる
        - 新人の導入がしやすい(タスクで困った時にも過去のverを参考したり、そもそもタスクの概要も掴みやすい)
        - MergeRequestで追加の議論もできる
    - デメリット
        - google系列に比べると作成は少々面倒(merge requestとかあるので)
        - git管理ができない人だと少し導入しづらい

## 決定
- とりあえず導入資料なので決定はしない、例としてこんな感じを想定していた。このような資料はプロジェクトが変わった際も積み重なるのでいい感じかな〜と思った。