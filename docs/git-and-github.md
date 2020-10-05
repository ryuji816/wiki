# Git and GitHub

## GitとGitHubの違い

Gitは分散型のバージョン管理を行うソフトウェアのことで，GitHubはGitで利用するリモートリポジトリをホスティングするなど他にも様々な機能を有したWebサービスのこと．Gitを利用したサービスはGitHub以外にも[GitLab](https://about.gitlab.com/)や[Bitbucket](https://bitbucket.org/product)などがある．

### Git

Gitは分散型のバージョン管理を行うソフトウェアで，Linuxを作成したLinus TorvaldsがLinux Kernelのバージョン管理用に作成したOSS．

- 以下のどちらかは必読
  - [サル先生のGit入門〜バージョン管理を使いこなそう〜【プロジェクト管理ツールBacklog】](https://backlog.com/ja/git-tutorial/)
  - [こわくない Git](https://www.slideshare.net/kotas/git-15276118)
  - [About - Git (英語)](https://git-scm.com/about)
- 上記記事では理解しきれなかった場合
  - [はじめてのGit - Speaker Deck](https://speakerdeck.com/d_hirayama/hazimetefalsegit)
  - [仕組みから理解する Git 入門 ~ ひとり開発でも便利 ~ - Speaker Deck](https://speakerdeck.com/mu_zaru/shi-zu-mikarali-jie-suru-git-ru-men-hitorikai-fa-demobian-li)


### GitHub

GitHubはGitの活用をよしなにするためのWebサービス．GitHub Actionsなどの機能追加もあり2020年現在GitHub以外のホスティングサービスを積極的に利用する理由はあまりないと思われる．GitHubの利用に関する入門は以下の記事を参照．

- 必読
  - [Hello World &middot; GitHub Guides](https://guides.github.com/activities/hello-world/)


## Gitの使い方

Gitでバージョン管理を行った開発では以下の流れを繰り返す．

1. GitHub上のリモートリポジトリを自身のアカウントにforkする
2. forkしたリポジトリをローカルにcloneする
3. 以降は以下の流れを繰り返す
    1. 作業用のブランチを作成する
    2. コードに変更を加える
    3. 変更したファイルをcommitする
    4. 複数のcommitを自身のリモートリポジトリにpushする
    5. GitHub上でPull Requestをfork元のリポジトリに対して行う
    6. コードレビューとその修正後自身のブランチの変更がfork元のリポジトリに取り込まれる
