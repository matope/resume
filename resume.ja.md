# 職務経歴書

## 基本情報

- 氏名: 後藤泰陽
- HN: 小野マトペ
- ID:
  - Twitter: [ono_matope](https://twitter.com/ono_matope)
  - GitHub: [matope](https://github.com/matope)
  - Blog: [小野マトペの納豆ペペロンチーノ日記](http://matope.hatenablog.com/)
  - Blog (old): [小野マトペの業務日誌\(アニメ制作してない篇\)](https://ono-matope.hatenadiary.jp/)
  - Qiita: [ono_matope](https://qiita.com/ono_matope)
- 出身大学: 法政大学情報科学部
- 生年: 1984

## 業務外活動

- 2007年〜 学生時代、Webサービス「ふぁぼったー」を開発(現在はクローズ済み)
  - いいね(favorite)がついたTweetをクロールして集計するWebサイト
  - 当時は自分のツイートへの反応を知る手段がなかったこともあり、人気のサービスに
  - レンタルサーバーで負荷が捌き切れず、3台の自宅サーバーで Apache/PHP/Perl/MySQL で運用
  - ピーク時1000万/月以上のPVを記録

## 職務経歴

### ヤフー株式会社 (2008/4 - )

- 2008年、ヤフー入社。システム統括本部でID関連システムの開発に関わるが、2009年下半期にオブジェクトストレージの内製プロジェクトの立ち上げに参加。参加2年目以降はコア部分の設計に携わる。
- 2012年ごろ、分散KVS (いわゆるNoSQL)データベースの導入プロジェクトの立ち上げに参加。OSSの分散データベースの性能検証などを担当。Apache Cassandraの導入後はクラスタ運用上のトラブルシューティングなどをサポート。
- 2014年ごろ、次世代のオブジェクトストレージ Dragon の企画を立案。承認され、少人数チームのテックリードとして設計・開発を担う。
    - Go言語と Cassandra を使い、S3互換API を提供するコンセプトを決定。
    - 2016年1月にローンチ。以降も安全性やパフォーマンスの改善に取り組む。ヤフーのほとんどのサービスから利用され、2017年11月時点で200億個、11ペタバイトのオブジェクトを安定してストア。
-  2018年下半期、他部署に異動。Webセキュリティ関連ライブラリの保守担当に配属

### メルペイ (2019/09 - )

- 2019年メルペイに入社、IDプラットフォームに配属
  - [mercari/go\-circuitbreaker](https://github.com/mercari/go-circuitbreaker) を開発。（[解説](https://speakerdeck.com/matope/mercari-dot-go-number-12-go-circuitbreakerfalsegoshao-jie)）

### フリーランス(2021/1 - )

- 2020年にメルペイを退社。2021年からフリーランス

以上

## 公開資料

### Go
- slide: [context パッケージの紹介](https://go-talks.appspot.com/github.com/matope/talks/2016/context/context.slide#1) (個人としての登壇) (2016/08/08)
  - [Go 1.7 Release Party in Tokyo](https://gocon.connpass.com/event/37332/) にて、新パッケージの context の意義と使い方を解説した。
- [mercari\.go \#12 go\-circuitbreakerのご紹介 \- Speaker Deck](https://speakerdeck.com/matope/mercari-dot-go-number-12-go-circuitbreakerfalsegoshao-jie)
  - 2019年12月6日 mercari.go #12 にて

### Cassandra

- slide: [Cassandra Summit 2016 注目セッション報告](https://www.slideshare.net/techblogyahoo/cassandra-summit-2016) (2016/10/12)
  - Cassandra meetup in Tokyo, Fall 2016 にて、 Cassandra Summit 2016の参加報告を発表した。Cassandra 3.0におけるストレージエンジン改良に関する主な発表を紹介した(p.6-p.34)。

### Dragon

- slide: [Goでヤフーの分散オブジェクトストレージを作った話 Go Conference 2017 Spring](https://www.slideshare.net/techblogyahoo/go-go-conference-2017-spring) (2017/03/25)
  - Go Conference 2017 Spring にて、オブジェクトストレージ Dragon をGo言語で開発した事例といくつかの技術的な工夫について紹介した。
- slide: [Dragon: A Distributed Object Storage at Yahoo\! JAPAN \(WebDB Forum 201…](https://www.slideshare.net/techblogyahoo/dragon-a-distributed-object-storage-at-yahoo-japan-webdb-forum-2017) (2017/09/19)
  - お茶の水大学にて開催された WebDB Forum 2017 にて登壇し、オブジェクトストレージ Dragon のアーキテクチャを紹介した。
- blog: [ヤフーの分散オブジェクトストレージ Dragon について \- Yahoo\! JAPAN Tech Blog](https://techblog.yahoo.co.jp/architecture/dragon-object-storage-architecture/) (2017/10/12)
  - WebDB Forum での発表資料をもとに、ヤフーのテックブログ上でDragon のアーキテクチャをくわしく解説する記事を公開した。

## OSS活動

### Go言語

- net/http の http.Client に Expect:100-continue 仕様のサポートを追加。Go1.6にマージ。(2016/05/15)
    - Ticket: [net/http: Client support for Expect: 100\-continue · Issue \#3665 · golang/go](https://github.com/golang/go/issues/3665)
- go get のGithub Enterprise 対応に関するIssue を報告 (2016/11/12)
    - GHE上のリポジトリのサブディレクトリを go get できない問題を報告。最終的にGitHub Enterprise側で対策され解決した。(2018/03/28)
    - Ticket: [cmd/go: add support for GitHub Enterprise import path · Issue \#17898 · golang/go](https://github.com/golang/go/issues/17898)

### Cassandra

- 巨大なパーティションに対する SELECT のレイテンシを40%程度改善した (2016/10/04)
    - Ticket: [\[CASSANDRA\-12731\]](https://issues.apache.org/jira/browse/CASSANDRA-12731)
    - Cassandra 3.10 にマージ
    - パッチ作成中に発見したコンパクションのバグも[あわせて修正した](https://issues.apache.org/jira/browse/CASSANDRA-12717)。
- クエリのトレース記録に、プリペアドステートメントのCQL文を含めるようする改修 (2016/05/06)
    - Dragonのパフォーマンスチューニング中に必要になり実装した。
    - Ticket: [\[CASSANDRA\-11425\]](https://issues.apache.org/jira/browse/CASSANDRA-11425)
    - Cassandra 3.8 にマージ。
- Cassandra 3.0 系へのupgrade中に発生した深刻なデータ破損バグの調査・レポート (2017/03/17)
    - 社内の開発用クラスタをアップグレード中に発見したデータ破損を社内エンジニア数人で調査し、粘り強く再現手順を見つけ報告した。Issueは優先度「緊急」にて対応され、 Cassandra 3.0.10, 3.0.11 へマージされた。
    - Ticket: [CASSANDRA\-13125](https://issues.apache.org/jira/browse/CASSANDRA-13125), [CASSANDRA\-13320](https://issues.apache.org/jira/browse/CASSANDRA-13320)

### その他

- gocql
    - Go言語のCassandraドライバ gocqlに対してバグ修正、機能追加など9件のコントリビューションを行った
        - Tickets:[Pull Requests · gocql/gocql](https://github.com/gocql/gocql/pulls?utf8=%E2%9C%93&q=author%3Amatope)
- circuitbreaker
    - Go言語の Circuit Breakerライブラリである rubyist/circuitbreaker に、Context対応など2件のコントリビューションを行なった。
        - Tickets: [Pull Requests · rubyist/circuitbreaker](https://github.com/rubyist/circuitbreaker/pulls?q=is%3Apr+author%3Amatope+is%3Aclosed)

# 個人の技術的アウトプット

- ブログ
    - [gorilla/csrf で安全なWebフォームを作る \- 小野マトペの納豆ペペロンチーノ日記](http://matope.hatenablog.com/entry/2019/06/05/144435)
    - [ざっくり理解するPaxos \- 小野マトペの納豆ペペロンチーノ日記](http://matope.hatenablog.com/entry/2018/05/13/204749)
    - [GoとgRPCでKVS的なものを作ってみた \- 小野マトペの納豆ペペロンチーノ日記](http://matope.hatenablog.com/entry/2016/01/05/003234)
    - [RFC的に、HTTPヘッダってどんな値を使えるんでしたっけ？のメモ \- 小野マトペの納豆ペペロンチーノ日記](http://matope.hatenablog.com/entry/2015/08/01/192412)
    - [Dynamoの論文を訳した \- 小野マトペの納豆ペペロンチーノ日記](http://matope.hatenablog.com/entry/2012/05/11/143638)
- Qiita
    - [Goの文字列結合のパフォーマンス \- Qiita](https://qiita.com/ono_matope/items/d5e70d8a9ff2b54d5c37)
    - [Goのencoding/xmlを使いこなす \- Qiita](https://qiita.com/ono_matope/items/70080cc33b75152c5c2a)
    - [Goでnet/httpを使う時のこまごまとした注意 \- Qiita](https://qiita.com/ono_matope/items/60e96c01b43c64ed1d18)
    - [LevelDBの設計ドキュメント和訳 \- Qiita](https://qiita.com/ono_matope/items/f4c248d926f854f9034d)
    - [JSON Web Encryption \(JWE\) の解説 \- Qiita](https://qiita.com/ono_matope/items/938a98fb111a297b68b9)
- zenn
    - [退屈なURLクエリパースは gorilla/schema にやらせよう](https://zenn.dev/ono_matope/articles/b39f969cfa1754)

# スキル・経験・得意なこと

- スキルセット
    - 6年間のGo言語経験（とても得意）
    - Cassandra NoSQLデータベース（とても得意）
    - 英語 TOEIC IPテスト780点 (気を使ってくれる相手なら意思疎通可能)
    - C++/Java/PHP/MySQL による開発経験（…があるので対応はできますが得意というほどではない）
- 経験
    - 学生時代から数年間にわたるWebサービスの自主開発・運営経験
    - 高速・スケーラブル・高堅牢性の分散ストレージを企画し、設計・開発した経験
    - Go言語で大規模アプリケーションを開発した経験
    - Cassandra 等のNoSQLデータベースの運用者・利用者双方としての経験
- 得意なこと
    - 課題をシンプルに捉えること。チームで問題を共有し、粘り強く問題解決にアプローチすること
