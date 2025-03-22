# Model Context Protocol サーバー

このリポジトリは [Model Context Protocol](https://modelcontextprotocol.io/) (MCP) の*リファレンス実装*のコレクションであり、コミュニティによって構築されたサーバーと追加リソースへの参照も含まれています。

このリポジトリのサーバーは MCP の汎用性と拡張性を示し、大規模言語モデル（LLM）にツールやデータソースへの安全で制御されたアクセスを提供する方法を実証しています。
各 MCP サーバーは [Typescript MCP SDK](https://github.com/modelcontextprotocol/typescript-sdk) または [Python MCP SDK](https://github.com/modelcontextprotocol/python-sdk) を使用して実装されています。

> 注：このREADMEのリストは、新しい項目を追加する際のマージ競合を最小限に抑えるためにアルファベット順で維持されています。

## 🌟 リファレンスサーバー

これらのサーバーは MCP の機能と TypeScript および Python SDK を示すことを目的としています。

- **[AWS KB Retrieval](src/aws-kb-retrieval-server)** - Bedrock Agent Runtime を使用した AWS Knowledge Base からの検索
- **[Brave Search](src/brave-search)** - Brave の検索 API を使用したウェブおよびローカル検索
- **[EverArt](src/everart)** - 様々なモデルを使用した AI 画像生成
- **[Everything](src/everything)** - プロンプト、リソース、ツールを備えたリファレンス/テストサーバー
- **[Fetch](src/fetch)** - LLM の効率的な使用のためのウェブコンテンツ取得と変換
- **[Filesystem](src/filesystem)** - 設定可能なアクセス制御を備えた安全なファイル操作
- **[Git](src/git)** - Git リポジトリの読み取り、検索、操作のためのツール
- **[GitHub](src/github)** - リポジトリ管理、ファイル操作、GitHub API 統合
- **[GitLab](src/gitlab)** - プロジェクト管理を可能にする GitLab API
- **[Google Drive](src/gdrive)** - Google Drive のファイルアクセスと検索機能
- **[Google Maps](src/google-maps)** - 位置情報サービス、ルート案内、場所の詳細情報
- **[Memory](src/memory)** - ナレッジグラフベースの永続的メモリシステム
- **[PostgreSQL](src/postgres)** - スキーマ検査を備えた読み取り専用データベースアクセス
- **[Puppeteer](src/puppeteer)** - ブラウザの自動化とウェブスクレイピング
- **[Redis](src/redis)** - Redis キーバリューストアとの対話
- **[Sentry](src/sentry)** - Sentry.io からの問題の取得と分析
- **[Sequential Thinking](src/sequentialthinking)** - 思考シーケンスを通じた動的で反射的な問題解決
- **[Slack](src/slack)** - チャンネル管理とメッセージング機能
- **[Sqlite](src/sqlite)** - データベース操作とビジネスインテリジェンス機能
- **[Time](src/time)** - 時間とタイムゾーン変換機能

## 🤝 サードパーティサーバー

### 🎖️ 公式統合

公式統合は、自社プラットフォーム向けに本番環境対応の MCP サーバーを構築している企業によって管理されています。

- <img height="12" width="12" src="https://www.21st.dev/favicon.ico" alt="21st.dev Logo" /> **[21st.dev Magic](https://github.com/21st-dev/magic-mcp)** - 最高の 21st.dev デザインエンジニアに触発されたクラフトUIコンポーネントを作成
- <img height="12" width="12" src="https://invoxx-public-bucket.s3.eu-central-1.amazonaws.com/frontend-resources/adfin-logo-small.svg" alt="Adfin Logo" /> **[Adfin](https://github.com/Adfin-Engineering/mcp-server-adfin)** - 支払いに必要な唯一のプラットフォーム - すべての支払いを一箇所で管理し、[Adfin](https://www.adfin.com/) による請求書発行と会計照合を行います
- <img height="12" width="12" src="https://www.agentql.com/favicon/favicon.png" alt="AgentQL Logo" /> **[AgentQL](https://github.com/tinyfish-io/agentql-mcp)** - [AgentQL](https://www.agentql.com/) を使用して AI エージェントが非構造化ウェブから構造化データを取得できるようにします
- <img height="12" width="12" src="https://agentrpc.com/favicon.ico" alt="AgentRPC Logo" /> **[AgentRPC](https://github.com/agentrpc/agentrpc)** - [AgentRPC](https://www.agentrpc.com/) を使用してネットワーク境界を越えてあらゆる関数、あらゆる言語に接続します
- <img height="12" width="12" src="https://aiven.io/favicon.ico" alt="Aiven Logo" /> **[Aiven](https://github.com/Aiven-Open/mcp-aiven)** - [Aiven プロジェクト](https://go.aiven.io/mcp-server)をナビゲートし、PostgreSQL®、Apache Kafka®、ClickHouse®、OpenSearch® サービスと対話します
- <img height="12" width="12" src="https://apify.com/favicon.ico" alt="Apify Logo" /> **[Apify](https://github.com/apify/actors-mcp-server)** - [Actors MCP Server](https://apify.com/apify/actors-mcp-server): 3,000以上の事前構築されたクラウドツールを使用して、ウェブサイト、Eコマース、ソーシャルメディア、検索エンジン、地図などからデータを抽出します
- <img height="12" width="12" src="https://resources.audiense.com/hubfs/favicon-1.png" alt="Audiense Logo" /> **[Audiense Insights](https://github.com/AudienseCo/mcp-audiense-insights)** - [Audiense](https://www.audiense.com/products/audiense-insights) レポートからのマーケティングインサイトとオーディエンス分析（人口統計、文化、インフルエンサー、コンテンツエンゲージメント分析を含む）
- <img height="12" width="12" src="https://axiom.co/favicon.ico" alt="Axiom Logo" /> **[Axiom](https://github.com/axiomhq/mcp-server-axiom)** - 自然言語でAxiomのログ、トレース、その他すべてのイベントデータをクエリおよび分析
- <img height="12" width="12" src="https://www.bankless.com/favicon.ico" alt="Bankless Logo" /> **[Bankless Onchain](https://github.com/bankless/onchain-mcp)** - ERC20トークン、トランザクション履歴、スマートコントラクトの状態などのオンチェーンデータのクエリを実行

### 🌎 コミュニティサーバー

コミュニティによって開発・維持されているサーバーの拡大セットは、さまざまな領域における MCP のさまざまな応用を実証しています。

> **注意:** コミュニティサーバーは**テストされていない**ため、**自己責任**で使用してください。これらは Anthropic と提携したり、承認されたりしているものではありません。

(※コミュニティサーバーの詳細なリストはここでは省略されています。オリジナルの英語版 README.md を参照してください)

## 📚 フレームワーク

これらは MCP サーバーやクライアントを構築しやすくする高レベルのフレームワークです。

### サーバー向け

- **[EasyMCP](https://github.com/zcaceres/easy-mcp/)** (TypeScript)
- **[FastAPI to MCP auto generator](https://github.com/tadata-org/fastapi_mcp)** – **[Tadata](https://tadata.com/)** による FastAPI エンドポイントを MCP ツールとして自動的に公開するためのゼロ設定ツール
- **[FastMCP](https://github.com/punkpeye/fastmcp)** (TypeScript)
- **[Foxy Contexts](https://github.com/strowk/foxy-contexts)** – **[strowk](https://github.com/strowk)** による Golang で MCP サーバーを構築するためのライブラリ
- **[MCP-Framework](https://mcp-framework.com)** Typescript で簡単かつ迅速に MCP サーバーを構築。`mcp create app` でプロジェクトを作成する CLI も付属。**[Alex Andru](https://github.com/QuantGeekDev)** により、5分以内に最初のサーバーを立ち上げることができます
- **[Quarkus MCP Server SDK](https://github.com/quarkiverse/quarkus-mcp-server)** (Java)
- **[Template MCP Server](https://github.com/mcpdotdirect/template-mcp-server)** - TypeScript サポート、デュアルトランスポートオプション、拡張可能な構造を備えた新しい Model Context Protocol サーバープロジェクトを作成するための CLI ツール

### クライアント向け

- **[codemirror-mcp](https://github.com/marimo-team/codemirror-mcp)** - リソースメンションとプロンプトコマンドのための Model Context Protocol (MCP) を実装する CodeMirror 拡張機能

## 📚 リソース

MCP に関する追加リソース。

- **[AiMCP](https://www.aimcp.info)** - **[Hekmon](https://github.com/hekmon8)** による適切な MCP ツールを見つけるための MCP クライアントとサーバーのコレクション
- **[Awesome Crypto MCP Servers by badkk](https://github.com/badkk/awesome-crypto-mcp-servers)** - **[Luke Fan](https://github.com/badkk)** によるキュレーションされた MCP サーバーのリスト
- **[Awesome MCP Servers by appcypher](https://github.com/appcypher/awesome-mcp-servers)** - **[Stephen Akinyemi](https://github.com/appcypher)** によるキュレーションされた MCP サーバーのリスト
- **[Awesome MCP Servers by punkpeye](https://github.com/punkpeye/awesome-mcp-servers)** (**[website](https://glama.ai/mcp/servers)**) - **[Frank Fiegel](https://github.com/punkpeye)** によるキュレーションされた MCP サーバーのリスト
- **[Awesome MCP Servers by wong2](https://github.com/wong2/awesome-mcp-servers)** (**[website](https://mcpservers.org)**) - **[wong2](https://github.com/wong2)** によるキュレーションされた MCP サーバーのリスト
- **[Discord Server](https://glama.ai/mcp/discord)** – **[Frank Fiegel](https://github.com/punkpeye)** による MCP 専用のコミュニティ Discord サーバー
- **[Discord Server (ModelContextProtocol)](https://discord.gg/jHEGxQu2a5)** – **[Alex Andru](https://github.com/QuantGeekDev)** による Model Context Protocol に特化したアクティブな Discord コミュニティで、開発者と繋がり、洞察を共有し、プロジェクトで協力する

- **[MCP Badges](https://github.com/mcpx-dev/mcp-badges)** – **[Ironben](https://github.com/nanbingxyz)** による明確で目を引くバッジであなたの MCP プロジェクトを素早くハイライト
- **[MCP Servers Hub](https://github.com/apappascs/mcp-servers-hub)** (**[website](https://mcp-servers-hub-website.pages.dev/)**) - **[apappascs](https://github.com/apappascs)** によるキュレーションされた MCP サーバーのリスト
- **[MCP X Community](https://x.com/i/communities/1861891349609603310)** – **[Xiaoyi](https://x.com/chxy)** による MCP のための X コミュニティ
- **[mcp-cli](https://github.com/wong2/mcp-cli)** - **[wong2](https://github.com/wong2)** による Model Context Protocol のための CLI インスペクター
- **[mcp-get](https://mcp-get.com)** - **[Michael Latman](https://github.com/michaellatman)** による MCP サーバーのインストールと管理のためのコマンドラインツール
- **[mcp-guardian](https://github.com/eqtylab/mcp-guardian)** - **[EQTY Lab](https://eqtylab.io)** による MCP サーバーのプロキシ/管理制御のための GUI アプリケーション + ツール
- **[mcp-manager](https://github.com/zueai/mcp-manager)** - **[Zue](https://github.com/zueai)** による Claude Desktop 用 MCP サーバーのインストールと管理のためのシンプルな Web UI
- **[MCPHub](https://github.com/Jeamee/MCPHub-Desktop)** – **[Jeamee](https://github.com/jeamee)** による MCP サーバーの発見、インストール、管理のためのオープンソースの MacOS & Windows GUI デスクトップアプリ
- **[mcp.run](https://mcp.run)** - 安全でポータブルな MCP サーバーをインストール・実行するためのホスト型レジストリおよび制御プレーン
- **[mcp-dockmaster](https://mcp-dockmaster.com)** - Windows、Linux、MacOS 用の MCP サーバーをインストールおよび管理するためのオープンソース UI
- <img height="12" width="12" src="https://mkinf.io/favicon-lilac.png" alt="mkinf Logo" /> **[mkinf](https://mkinf.io)** - AI エージェントワークフローを加速するためのホスト型 MCP サーバーのオープンソースレジストリ
- **[Open-Sourced MCP Servers Directory](https://github.com/chatmcp/mcp-directory)** - **[mcpso](https://mcp.so)** によるキュレーションされた MCP サーバーのリスト
- <img height="12" width="12" src="https://opentools.com/favicon.ico" alt="OpenTools Logo" /> **[OpenTools](https://opentools.com)** - **[opentoolsteam](https://github.com/opentoolsteam)** による MCP サーバーの検索、インストール、構築のためのオープンレジストリ
- **[PulseMCP](https://www.pulsemcp.com)** ([API](https://www.pulsemcp.com/api)) - **[Tadas Antanavicius](https://github.com/tadasant)**、**[Mike Coughlin](https://github.com/macoughl)**、**[Ravina Patel](https://github.com/ravinahp)** による MCP サーバー、クライアント、記事、ニュースを発見するためのコミュニティハブ＆ウィークリーニュースレター
- **[r/mcp](https://www.reddit.com/r/mcp)** – **[Frank Fiegel](https://github.com/punkpeye)** による MCP 専用の Reddit コミュニティ
- **[r/modelcontextprotocol](https://www.reddit.com/r/modelcontextprotocol)** – Model Context Protocol コミュニティの Reddit ページ - アイデアを議論し、質問への回答を得て、同じ考えを持つ人々とネットワークを作り、プロジェクトを紹介しましょう！by **[Alex Andru](https://github.com/QuantGeekDev)**

- **[Smithery](https://smithery.ai/)** - **[Henry Mao](https://github.com/calclavia)** による LLM エージェント用の適切なツールを見つけるための MCP サーバーレジストリ
- **[Toolbase](https://gettoolbase.ai)** - **[gching](https://github.com/gching)** によるコーディング不要でわずか数クリックでツールと MCP サーバーを管理するデスクトップアプリケーション

## 🚀 はじめに

### このリポジトリの MCP サーバーを使用する
このリポジトリの TypeScript ベースのサーバーは `npx` で直接使用できます。

例えば、次のコマンドで [Memory](src/memory) サーバーを起動できます：
```sh
npx -y @modelcontextprotocol/server-memory
```

このリポジトリの Python ベースのサーバーは [`uvx`](https://docs.astral.sh/uv/concepts/tools/) または [`pip`](https://pypi.org/project/pip/) で直接使用できます。使いやすさとセットアップのしやすさから `uvx` が推奨されています。

例えば、次のコマンドで [Git](src/git) サーバーを起動できます：
```sh
# uvx を使用する場合
uvx mcp-server-git

# pip を使用する場合
pip install mcp-server-git
python -m mcp_server_git
```

`uv` / `uvx` のインストールには[これらの](https://docs.astral.sh/uv/getting-started/installation/)指示に従い、`pip` のインストールには[これらの](https://pip.pypa.io/en/stable/installation/)指示に従ってください。

### MCP クライアントを使用する
ただし、サーバー単体で実行してもあまり役に立たず、代わりに MCP クライアントに設定する必要があります。例えば、上記のサーバーを使用するための Claude Desktop 設定は次のようになります：

```json
{
  "mcpServers": {
    "memory": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-memory"]
    }
  }
}
```

MCP クライアントとして Claude Desktop を使用する追加例は次のようになります：

```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-filesystem", "/path/to/allowed/files"]
    },
    "git": {
      "command": "uvx",
      "args": ["mcp-server-git", "--repository", "path/to/git/repo"]
    },
    "github": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-github"],
      "env": {
        "GITHUB_PERSONAL_ACCESS_TOKEN": "<YOUR_TOKEN>"
      }
    },
    "postgres": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-postgres", "postgresql://localhost/mydb"]
    }
  }
}
```

## 🛠️ 自分自身のサーバーを作成する

独自の MCP サーバーの作成に興味がありますか？ MCP サーバーの実装に関する包括的なガイド、ベストプラクティス、技術的な詳細については、[modelcontextprotocol.io](https://modelcontextprotocol.io/introduction) の公式ドキュメントをご覧ください。

## 🤝 貢献

このリポジトリへの貢献に関する情報は [CONTRIBUTING.md](CONTRIBUTING.md) を参照してください。

## 🔒 セキュリティ

セキュリティの脆弱性の報告については [SECURITY.md](SECURITY.md) を参照してください。

## 📜 ライセンス

このプロジェクトは MIT ライセンスの下でライセンスされています - 詳細は [LICENSE](LICENSE) ファイルを参照してください。

## 💬 コミュニティ

- [GitHub Discussions](https://github.com/orgs/modelcontextprotocol/discussions)

## ⭐ サポート

MCP サーバーが役立つと思われる場合は、リポジトリにスターを付け、新しいサーバーや改善点を貢献することを検討してください！

---

Anthropic によって管理されていますが、コミュニティと共に構築されています。Model Context Protocol はオープンソースであり、誰もが独自のサーバーや改善点を貢献することを奨励しています！
