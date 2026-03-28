# copilot-md-example
GitHub Copilot MD example

## 1. Always-on

### .github/copilot-instructions.md
- GitHub Copilot 専用の常時適用指示ファイル
- `.github/copilot-instructions/` ディレクトリに複数ファイルを置く形式でも適用可能

### AGENTS.md
- 複数の AI Coding Agent が参照する汎用指示ファイル
- ルートに1つ、またはサブディレクトリにネストして適用可能

### CLAUDE.md
- Claude Code 専用の常時適用指示ファイル
- ルートに1つ、またはサブディレクトリにネストして適用可能

### GEMINI.md
- Gemini CLI 専用の常時適用指示ファイル
- ルートに1つ、またはサブディレクトリにネストして適用可能

## 2. Path-specific

### .github/instructions/*.instructions.md
- GitHub Copilot 専用のパス固有指示ファイル
- frontmatter の `applyTo` でファイルパターンを指定し、特定のファイルにのみ適用可能

## 3. Custom-Agent

### .github/agents/*.agent.md
- GitHub Copilot 専用のカスタムエージェント定義ファイル
- Copilot Chat で `@agent-name` として呼び出し可能

## 4. wip

### .github/prompts/*.prompt.md
- wip
