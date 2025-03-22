# MCP Server Setup Guide

## Configuration

### MCP Settings Location

設定ファイルは以下の場所にあります：

- Cursor用: `~/Library/Application Support/Cursor/User/globalStorage/saoudrizwan.claude-dev/settings/cline_mcp_settings.json`
- Claude Desktop用: `~/Library/Application Support/Claude/claude_desktop_config.json`

### Volta環境での設定例

macOSでVoltaを使用している場合、以下の設定が動作します：

```json
{
  "mcpServers": {
    "github.com/modelcontextprotocol/servers/tree/main/src/github": {
      "command": "/Users/username/.volta/bin/npx",
      "args": [
        "-y",
        "@modelcontextprotocol/server-github"
      ],
      "env": {
        "GITHUB_PERSONAL_ACCESS_TOKEN": "<YOUR_TOKEN>"
      },
      "disabled": false,
      "autoApprove": []
    }
  }
}
```

### トラブルシューティング

#### 失敗したパターン

1. `node` コマンドを直接使用
```json
{
  "command": "node",
  "args": [
    "/path/to/server-github/build/index.js"
  ]
}
```
エラー: `spawn node ENOENT`

2. `volta` コマンドを使用
```json
{
  "command": "/Users/username/.volta/bin/volta",
  "args": [
    "run",
    "node",
    "/path/to/server-github/build/index.js"
  ]
}
```
エラー: 接続タイムアウト

#### 成功したパターン

Voltaの `npx` へのフルパスを使用することで解決：
```json
{
  "command": "/Users/username/.volta/bin/npx",
  "args": [
    "-y",
    "@modelcontextprotocol/server-github"
  ]
}
```

## 動作確認

サーバーが正しく設定されているか確認するには、以下のような操作を試してください：

```typescript
// リポジトリ検索
{
  "query": "modelcontextprotocol",
  "page": 1,
  "perPage": 5
}
```

正常に結果が返ってくれば、設定は成功です。
