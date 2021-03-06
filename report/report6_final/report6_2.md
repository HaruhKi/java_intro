# 課題レポート6: Java最終課題（小作品制作、仕上げ）について

- ＜目次＞
  - <a href="#conditions">条件</a>
  - <a href="#example">課題設計例</a>
  - <a href="#report">レポートに含めるべき内容</a>
  - 参考: <a href="#eval">主な評価項目</a>
  - <a href="#submit">提出方法</a>
  - <a href="#oral">口頭試問</a>

<hr>

## <a name="conditions">条件</a>
- 一般条件
  - Java言語でコーディングすること。
    - 一人当たり100行以上。2,3人の場合、話し合う時間、コード共有部分、github上でのマージ等といった負担もかかってくるため、一人あたり約80行（2人なら合計160行程度）でもok。どこを担当したのか明示すること。
      - 2,3人で取り組む場合、口頭試問（レポートについて口頭で説明）を必須とします。（後述）
  - package指定すること。
    - 1人で取り組む場合、``jp.ac.uryukyu.ie.e1857xx`` 形式で指定すること。
    - 2,3人で取り組む場合、``jp.ac.uryukyu.ie.e185701_e185720`` のように、アカウントの若い番号から順にアンダースコアで結合したパッケージ名とすること。
  - 開発は Git + GitHub を利用すること。（commit log が最終版の1件しかないのはNG。メソッド単位なり適度なタイミングでcommitしよう。）
  - JavaDoc形式でクラス、メソッドにドキュメントを書くこと。
  - JUnitでユニットテストを記述すること。
  - Gradleで、
    - 実行可能なjarファイルを生成できるようにすること。
    - JUnitで記述したテストを実行できるようにすること。
  - (README.mdというファイル名で、概要説明をするとベター。)
- 最低3クラス作成すること。
  - **クラス1: 課題を解決するクラス（クラスは複数でもかまわない）。**
    - 便宜上以下ではSolverと呼ぶ。実際には適切なクラス名を付けること。
    - Solverクラスには、2個以上の自作メソッドを含むこと。
    - 後述のクラス2に、1つ以上のユニットテストを書くこと。
  - **クラス2: SolverのメソッドをユニットテストするためのSolverTestクラス。**
    - SolverTestのクラス名は適切に付けること。
  - **クラス3: Solverを動かすためのMainクラス。**
    - 原則としてmainメソッドだけとしよう。
  - 全クラス共通ルール
    - 1つのメソッドは50行を超えないこと。

<hr>

## <a name="example">課題設計例</a>
- 前述の条件を守っているなら、何を実装しても構わない。以下は課題例の紹介。
- 具体的な課題例
  - 五目並べを実装してみよう。
  - オセロを実装してみよう。
  - ポーカーを実装してみよう。
  - （指定したディレクトリ内にあるテキストファイルを対象とする）検索エンジンを実装してみよう。
  - 上記を簡略化した小さい課題を設定して、実装してみよう。

<hr>

## <a name="report">レポートに含めるべき内容</a>
- 大前提
  - **開発途中段階でのレポートとなっても構わない。tryした過程がわかるように報告しよう**。レポート作成には時間がかかるのは身をもって体験しているはずだ。〆切数日前にはレポート作成に取り掛かろう。
  - ページ上限は設定しないが、目安は長くて10ページ程度。これ以上長くなりそうな場合、整理することを検討しよう。
- 含めるべき項目
  1. 表紙
    - タイトル: 「課題レポート6: Java最終課題（サブタイル）」
      - 設定した課題内容を端的に示すサブタイトルを付けよう。
    - 学籍番号、氏名
    - 協力者がいる場合、学籍番号＆氏名。
    - ペアやチームで取り組んだ場合、作業分担の明示。
  - GitHubリポジトリURL
    - GitHubにpushできない人は早めに相談すること。これがない場合、それだけで大幅減点します。
  - **課題説明: 自由課題であるため、設定した「課題内容」について十分説明すること。**
  - **取り組み方: 設定した課題について、どのように取り組んだのか述べること。**
  - **コード解説: 最低限、主要なメソッド1つについて十分に解説すること。**
    - 最終コードはGitHubにあるため、レポートに全コードを掲載する必要はない。解説したい場所に限定して、掲載コードを必要最小限に留めること。（解説のないコード掲載は無意味なので辞めよう）
  - 実行結果: 動作を確認できる実行結果を掲載すること。
  - 考察: 取り組みを通した気付きについて考察すること。

<hr>

## <a name="eval">参考: 主な評価項目</a>
- 以下、シラバスの達成目標より抜粋。
  - プログラミングの概念と設計方法を理解し，KISS原則を意識した構造化プログラミング(100行程度)を実践することができる。（小作品制作）
  - 第三者にとって保守管理し易くするためにコード規約を意識し，適切なコメントを記述，単体テストを用意することができる。（小作品仕上げ）

<hr>

## <a name="submit">提出方法</a>
- ソースファイルはGitHubにあるだけで良い。（**Googleドライブ上に提出されててもあっても見ません**）
- 提出物は「レポート」の1点である。
  - GitHubリポジトリを誤って削除しないように注意すること。（コードを確認できない場合、大幅減点となる）
  - ペアチームで取り組んでいる場合、
    - 個別レポートでもまとめて1レポートでも構わない。まとめる場合には誰がどこを書いたのかも明示するようにすること。
    - レポートの「提出先フォルダ名」は、アカウント名をソートして列挙すること。例えば「e185701+e185702」。間は+でも_でも区切りが分かるならOK。
- レポートは電子ファイルで提出するものとする。
- 提出先:
  - 「Google ドキュメント」のreport6。

<hr>

## <a name="oral">口頭試問</a>
- 2,3人で取り組む場合、口頭試問（レポートについて口頭で説明）を必須とします。
- 想定イメージ
  - まずレポート全体（コード全体）の概要と、役割分担について、数分程度で解説。これは誰がやっても良い。
  - 次に、担当毎に担当した箇所について説明。レポートやコードを示しながら（プロジェクタ等で投影しながら）説明して貰う予定。一人あたり5分程度。
  - これらを、全体や個別に質問しながら確認していく。
  - 全体に要する時間は、2名で長くて20分、3名で30分を想定。
