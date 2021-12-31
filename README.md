# For Code Competitions with Python
## 目的
- VS Code と開発コンテナで At Coder の問題を解く環境を構築します
- ローカル環境への影響を最小限にとどめます
## 前提
- docker の導入
- VS Code 及び以下の拡張機能の導入
   - Remote - Containers (ms-vscode-remote.remote-containers) 
- AtCoder との連携は https://github.com/kyuridenamida/atcoder-tools を利用します
## 使用方法
1. `docker-compose up [--build]` で開発コンテナを起動します
2. VS Code の [Remote Explorer] から開発コンテナに attach します
## フォルダ構成
- problems: このフォルダで `atcoder-tools gen {contest_id}` を実施し、問題をダウンロードします
- answer: 解き終わった問題を `{problem_id}_main.py` にリネームして保存します
   - problems/answer/ はgit管理されます