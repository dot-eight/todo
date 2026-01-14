
デプロイする

Github Pages

https://dot-eight.github.io/todo/

Vercel

https://todo-eta-mocha.vercel.app/

MCPを追加する

Playwright　MCP をプロジェクトに追加する

claude mcp add Playwright npx @Playwright/mcp@latest

Serena　MCP をプロジェクトに追加する

claude mcp add serena -- uvx --from git+https://github.com/oraios/serena serena-mcp-server --context
  ide-assistant --project $(pwd)
