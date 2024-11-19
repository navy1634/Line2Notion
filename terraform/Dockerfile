FROM hashicorp/terraform:latest

WORKDIR /terraform

# 必要なツールをインストール
RUN apk add --no-cache aws-cli

# フォルダをコピー
COPY . /terraform/

# エントリーポイントの設定
ENTRYPOINT ["terraform"]
