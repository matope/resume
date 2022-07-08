# Resume

(W.I.P.)

## Profile

- Name: Yasuharu Goto (後藤 泰陽)
- Birthday: 10/29/1984
- Education: Hosei University (Tokyo, Japan) 2004-2007
  - Bachelor of Computer Science
- Social media:
  - Twitter: [ono_matope](https://twitter.com/ono_matope)
  - GitHub: [matope](https://github.com/matope)
  - Blog: [小野マトペの納豆ペペロンチーノ日記](http://matope.hatenablog.com/)
  - Blog (old): [小野マトペの業務日誌\(アニメ制作してない篇\)](https://ono-matope.hatenadiary.jp/)
  - Qiita: [ono_matope](https://qiita.com/ono_matope)

## Summary

- Designed and developped a distributed Object Storage System at Yahoo! JAPAN using Go and Cassandra.
- 5 years of experience in Golang programming.
- Technical leadership experience (up to 6 members)
- Experience in developing / managing a web service personally.
- TOEIC score 780.

## Technical skills

- Language: Fluent in Go and working knowledge of C++, Java and PHP.
- Database: Fluent in Cassandra and working knowledge of MySQL.
- OS: Linux (Red Hat based)
- Extremely creative with problem solving skills.

## Work experience

### Yahoo! JAPAN (2008 - )

- Joined a project to develop a Object Storage as a jounior engineer. (2009-)
- Joined a project to introduce NoSQL distributed database to the company. I had some performance surveys for some Open Source database software. After the introduction of Cassandra, I supported trouble shootings to solve problems happen in the operation. (2012-)
- Designed and developped "Dragon" a new object storage as a tech lead of a small team (2014-).
    - After the launch in Jan 2016, continued to improve the product.
    - Dragon was storing over 11PB and 20Billion objects as at Nov 2017.

### Merpay (2019 - 2020)

- Joined to Merpay as an ID platform developer.
  - Released [mercari/go\-circuitbreaker](https://github.com/mercari/go-circuitbreaker) as an OSS（[detail](https://speakerdeck.com/matope/mercari-dot-go-number-12-go-circuitbreakerfalsegoshao-jie)）

### Freelance( 2021 - )

- Started working as an freelance engineer since 2021.

## Publications

### Go
- slide: [Introduction to context package](https://go-talks.appspot.com/github.com/matope/talks/2016/context/context.slide#1) (in Japanese / talk as a indivisual) (2016/08/08)
  - Introduced new package "context" that was introduced in Go1.7 at "Go1.7 Release Party in Tokyo".
- [mercari\.go \#12 go\-circuitbreakerのご紹介 \- Speaker Deck](https://speakerdeck.com/matope/mercari-dot-go-number-12-go-circuitbreakerfalsegoshao-jie)
  - at mercari.go #12 (December/06/2019)

### Cassandra

- slide: [Cassandra Summit 2016 注目セッション報告](https://www.slideshare.net/techblogyahoo/cassandra-summit-2016)  (in Japanese) (2016/10/12)
  - A participation report of Cassandra Summit 2016 at "Cassandra meetup in Tokyo, Fall 2016". I summarized and introduced a presentation on the improvements of storage engine in Cassandra 3.0.

### Dragon

- slide: [Developping Yahoo! JAPAN's distributed object storage in Go - Go Conference 2017 Spring](https://www.slideshare.net/techblogyahoo/go-go-conference-2017-spring) (3/25/2017)
  - Introduced our case in developing Distributed Object Storage called "Dragon" in Golang at Go Conference 2017 Spring. 

- slide: [Dragon: A Distributed Object Storage at Yahoo\! JAPAN \(WebDB Forum …](https://www.slideshare.net/techblogyahoo/dragon-a-distributed-object-storage-at-yahoo-japan-webdb-forum-2017-english-ver) (English version. 9/19/2017)
  - Introduced Dragon's architecture at WebDB Forum 2017 in Ochanomizu-Univ.
- blog: [ヤフーの分散オブジェクトストレージ Dragon について \- Yahoo\! JAPAN Tech Blog](https://techblog.yahoo.co.jp/architecture/dragon-object-storage-architecture/) (10/12/2017)
  - Published a blog post that share details of Dragon's architecture and considerations on Yahoo! JAPAN's tech-blog.

## Open Source Software contributions

### Go

- Add support for Expect:100-continue to Go's net/http client.
    - Merged to Go1.6 (5/15/2016)
    - Ticket: [net/http: Client support for Expect: 100\-continue · Issue \#3665 · golang/go](https://github.com/golang/go/issues/3665)
- Reported Github Enterprise support issue in go get. (11/12/2016)
    - Reported an issue that go get can not work with sub-directories in GHE. This issue has been solved by GHE team.
    - Ticket: [cmd/go: add support for GitHub Enterprise import path · Issue \#17898 · golang/go](https://github.com/golang/go/issues/17898)

### Cassandra

- Improved SELECT latency for large partitions by 40% (2016/10/04)
    - Ticket: [\[CASSANDRA\-12731\]](https://issues.apache.org/jira/browse/CASSANDRA-12731)
    - Merged in Cassandra 3.10.
    - Just small amount of code, but the removal of in-memory cache gained efficiency.
    - Also [fixed a bug](https://issues.apache.org/jira/browse/CASSANDRA-12717) in compaction process which I found in the work. 
- Add Prepared CQL statement to query trace records to improve traceability of query execution performance. (2016/05/06)
    - Ticket: [\[CASSANDRA\-11425\]](https://issues.apache.org/jira/browse/CASSANDRA-11425)
    - Merged in Cassandra 3.8。
- Investigated and reported a serious data-collapsing bug produced during upgrading to Cassandra 3.0. (3/17/2017)
    - Our team members including me patiently found a way to reproduce  the issue which was accidentally found in our cluster.
    - The issue was fixed  in priority "Urgent" by the Cassandra committers.
    - Ticket: [CASSANDRA\-13125](https://issues.apache.org/jira/browse/CASSANDRA-13125), [CASSANDRA\-13320](https://issues.apache.org/jira/browse/CASSANDRA-13320)

### others

- gocql
    - I made 9 ontributions which includes bug-fix and improvements to gocql an Cassandra driver for Go.
        - Tickets:[Pull Requests · gocql/gocql](https://github.com/gocql/gocql/pulls?utf8=%E2%9C%93&q=author%3Amatope)
- circuitbreaker
    - Had 2 contributions to circuitbreaker which is an Circuit Breaker library for Go including context support.
        - Tickets: [Pull Requests · rubyist/circuitbreaker](https://github.com/rubyist/circuitbreaker/pulls?q=is%3Apr+author%3Amatope+is%3Aclosed)


# Personal technical output

- In 2007, Launched a web service called "favotter" which is personally created. 
    - Which crawls and ranks "favorites" from Twitter.
    - Recorded 10M Page Views per month at the peek.
- Blog posts
    - [gorilla/csrf で安全なWebフォームを作る \- 小野マトペの納豆ペペロンチーノ日記](http://matope.hatenablog.com/entry/2019/06/05/144435)
    - [ざっくり理解するPaxos \- 小野マトペの納豆ペペロンチーノ日記](http://matope.hatenablog.com/entry/2018/05/13/204749)
    - [GoとgRPCでKVS的なものを作ってみた \- 小野マトペの納豆ペペロンチーノ日記](http://matope.hatenablog.com/entry/2016/01/05/003234)
    - [RFC的に、HTTPヘッダってどんな値を使えるんでしたっけ？のメモ \- 小野マトペの納豆ペペロンチーノ日記](http://matope.hatenablog.com/entry/2015/08/01/192412)
    - [Dynamoの論文を訳した \- 小野マトペの納豆ペペロンチーノ日記](http://matope.hatenablog.com/entry/2012/05/11/143638)
- Qiita articles
    - [Goの文字列結合のパフォーマンス \- Qiita](https://qiita.com/ono_matope/items/d5e70d8a9ff2b54d5c37)
    - [Goのencoding/xmlを使いこなす \- Qiita](https://qiita.com/ono_matope/items/70080cc33b75152c5c2a)
    - [Goでnet/httpを使う時のこまごまとした注意 \- Qiita](https://qiita.com/ono_matope/items/60e96c01b43c64ed1d18)
    - [LevelDBの設計ドキュメント和訳 \- Qiita](https://qiita.com/ono_matope/items/f4c248d926f854f9034d)
    - [JSON Web Encryption \(JWE\) の解説 \- Qiita](https://qiita.com/ono_matope/items/938a98fb111a297b68b9)
- zenn.dev articles
    - [退屈なURLクエリパースは gorilla/schema にやらせよう](https://zenn.dev/ono_matope/articles/b39f969cfa1754)
