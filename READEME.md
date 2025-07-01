# GitHub Copilot Rules
このリポジトリは、GitHub Copilotのルールをまとめたテンプレートです。

# 概要
本リポジトリでは、GitHub Copilotを使用する際のルールやガイドラインを提供します。これにより、開発者がCopilotを効果的に活用し、コードの品質とセキュリティを保つことができます。

## 設定集
### リポジトリのカスタム指示
[copilot-instructions.md](.github/copilot-instructions.md)では、リポジトリ全体に適用されるカスタム指示を定義しています。
これにより、Copilotが特定のプロジェクト要件に沿ったコードを生成するようになります。
利用時には、指示内容を確認し、必要に応じて調整してください。
また技術スタック、ディレクトリ構成、開発環境などの情報を明確に記載することで、Copilotがより適切なコードを提案できるようになります。

### プロンプトファイル
プロンプトファイルは、特定のタスクや機能に対する指示を提供します。
これにより、Copilotが特定の要件に基づいたコードを生成することができます。

作成済みプロンプトファイルは以下の通りです：
- [refactoring.prompt.md](.github/prompts/refactoring.prompt.md): コードのリファクタリングに関する指示を提供します。

### カスタムチャットモード
Github CopilotのデフォルトのチャットモードではAsk、Edit、Agentの3つのモードが用意されています。
本リポジトリでは、以下のカスタムチャットモードを定義しています。
- [taskmode.chatmode.md](.github/chatmodes/taskmode.chatmode.md): 開発前に技術的な調査と計画を行うためのタスクモードです。
  - ユーザの入力をもとに新しい機能や技術的な課題の概要を確認し、調査結果をもとにステップバイステップで実装計画を立てます。

### MCPの設定
[mcp.json](.github/mcp.json)は、GitHub Copilotで使用できるMCP（Model Configuration Profile）を定義しています。

一部のMCPは、npxを使用できない環境では動作しない場合があります。

### Github Copilotの設定
[settings.json](.github/settings.json)は、GitHub Copilotの設定を定義しています。
この設定ファイルは、Copilotの動作をカスタマイズするために使用されます。

現在は、以下の設定が含まれています：
- Next Edit Suggestionsの有効化
- コードの自動生成に関するプロンプト
- テストの自動生成に関するプロンプト
- コードレビューの自動生成に関するプロンプト
- コミットメッセージの自動生成に関するプロンプト
- プルリクエストの自動生成に関するプロンプト

## ライセンス
本リポジトリはMITライセンスのもとで公開されています。
詳細は[LICENSE](LICENSE)ファイルを参照してください。