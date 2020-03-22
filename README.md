# vscode-environment

## Docker ログインの方法
[GitHub Package RegistryのDockerイメージは認証無しではPullできない (2020/01/12時点) - Qiita](https://qiita.com/yoichiwo7/items/dcea47782a5189d1c1c9)
にあるように、公開レポジトリであっても、 GitHub Package Registry へのログインが必要。

1. https://github.com/settings/tokens で、適切な権限のパーソナルアクセストークンを発行する
2. docker login docker.pkg.github.com -u mur6 -p TOKEN でログインする

docker pull docker.pkg.github.com/mur6/vscode-environment/python:latest

で pull 出来るようになっている。

参考: [【GitHub】GitHub Package RegistryでDockerイメージを公開する（2019/10/27現在） - 開発覚書はてな版](https://kakkoyakakko2.hatenablog.com/entry/2019/10/27/003000)
