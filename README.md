# nextjs-app-router-sample

My First Next.js App Router App Sample

# 参考記事

こちらのチュートリアルを参考にしています。今後第 2 回も出るらしい

- https://codezine.jp/article/detail/17925?p=2

# アプリの内容

ソーシャルニュースサイト「Hacker News」の JSON Web API である、Hacker News API からデータを取得して、画面に表示する Web サイト

# 必要な通信処理

1. /topstories.json で 500 件分の記事 ID を取得する

2. 1 の先頭 20 件分の記事 ID を利用して、/item/<id> に 20 回アクセスして、左サイドメニューに表示するためのタイトルを入手する

3. 記事のページを開くまでに、/item/<id> にアクセスして記事のタイトルや本文を取得する

4. 記事データにはコメント ID のリストが含まれているので、コメント ID の 1 件ずつについて /item/<id> へのアクセスを行い、コメントデータを取得する（なおコメントの数は不定で、何回アクセスが発生するかはわからない）
