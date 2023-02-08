# Ansible

### Ansibleを用いて以下の構築を自動化

* EC2の構築
* RDSの構築
* ApacheサーバーにWordpressをデプロイ
* NginxサーバーにWordpressをデプロイ
* EC2にJupyter notebookをデプロイ
* EC2にGitlabをデプロイ(初期パスワード出力、設定パスワード出力)

### 使用方法

1. 実行したいタスクを`tasks`ディレクトリから選び、`main.yml`に`include_tasks`で指定。
1. `vars.yml`の変数を更新。
1. `hosts.ini`へマネージドノードを入力。
1. 以下のコマンドで実行。オプションで-vを付けると処理内容を出力。

__コマンド__

```
ansible-playbook -i hosts.ini main.yml
```