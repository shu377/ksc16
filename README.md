# ksc16 学生有志

2022/08/18 ~ 08/26 開催の第16回 KEK サマーチャレンジ (ksc16) 参加学生有志で活動記録を残そうと、非公式で活動しています。

$\LaTeX$ による分量無制限のレポートを主軸に掲載していきますが、解析データや回路図なんかも載せていこうと考えています。
補足すると、公式のレポートは Word で1人2ページです。

## ksc16 参加学生へ

以下の記述は当面の間頻繁に更新します。
特に執筆にあたり重大な変更事項はアナウンスしますが、細目は各自で適宜確認するようにしてください。

### $\LaTeX$ファイルのフォーマット

原則的にフォーマットは自由ですが、やたらめったらバラバラにならないように一部制限をかけます。

- documentclass は jsarticle を使用。
- 分類は `\section` 以下のみを使用。
- **ページ番号は削除**

ページ番号は $\LaTeX$ ファイルのプリアンブルに `\pagestyle{empty}` を書くことで消去できます。

> **INFO**
> 1ページ目だけページ番号が現れる事例があるようですが、その際は `\maketitle` の後で `\thispagestyle{empty}` とすると消えるようです。

また結合した際に不都合が生じた場合は個別に対応します。
原稿提出後も連絡は取れるようにしてください。

### git 運用にあたって

> **Note**
> 管理者から編集をお願いする方も含めて、各自必ずブランチを作成した上で作業してください。
> 運営も main ブランチに直接コミットを行うことは避けてください。

git の使い方は Google の情報が結構充実しています。
「GitHub 使い方」「gitとは」などと検索してもらえれば解決することが多いでしょう。
このリポジトリの [Wiki - Useful contents](https://github.com/LowToneVoice/ksc16/wiki/Useful-contents) には個人的に参考になったリンクなどをぶら下げてあります。
もし検索をかけても解決しない問題が発生した場合は個別に連絡してください。

運用は原則的に皆様の良識に委ねます。
後述「[個人情報について](#personal-info)」もご一読ください。
特にこちらで編集をお任せしている方をのぞき、他班のディレクトリを操作しないでください。

初めてプルリクエストを送る方は後述の[連絡先](#mail)に

- 氏名(本名)
- 班番号
- GitHub ユーザー名

を明記してメールしてください。
管理者をよくご存知の方、及び執筆に関する LINE グループに所属の方は LINE, slack, twitter DM, Discord などを使っていただいても構いません。

諸事情あって GitHub アカウントの取得が困難な方は個別に対応します。
データ送受信の利便性を考えて、[メール](#mail)または Slack でお問合せください。

### 命名規則

ルートディレクトリ ksc16 直下の階層では、各班 **"group + 班番号"** で統一してください。
管理者所属の7班のディレクトリはあらかじめ用意しておきましたので、それに倣ってください。
'group' と班番号の間にはスペースを入れないでください。

レポートはコンパイルして出来上がった **pdf ファイルを結合**して作成します。
group# ディレクトリに report ディレクトリを作って main.pdf を格納してください。
つまりこんな感じ。

```txt
ksc16
├── group1
│   ├── report
│   │   ├── main.tex
│   │   └── main.pdf
│   ├── img
... ...
└── report
    └── main.tex
```

編集にあたっては原則 report 内の main.pdf のみを参照して統合します。
report ディレクトリにはこれ以外にもファイルを入れてもらって結構です。

上記以外について、各班のディレクトリ内部について命名規則はありません。

### 個人情報について

<a id="personal-info">
</a>

ファイルをアップロードする際は、**ファイル内部に個人名などが残っていないか**、必ず確認してください。
コメントアウト部分の確認漏れには特にご注意ください。

Contributor と異なる個人名をファイルに意図的に残す場合は必ず本人の確認をとった上でお願いします。
その際、

- 本人の確認を取る
- 確認をとったことを[管理者に知らせる](#mail)

を徹底してください。
報告なく個人情報が掲載されている場合は、管理者側で予告なく削除することがあります。

## 連絡先

<a id="mail">管理者</a>
LowToneVoice
lowtonevoice@icloud.com

## 参考 url

第16回 大学生・高専生のための素粒子・原子核スクール サマーチャレンジ <https://www2.kek.jp/ksc/>

KEK_サマーチャレンジ twitter <https://twitter.com/kek_sc_sns>
