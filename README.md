# copilot-md-example
GitHub Copilot MD example

## 1. Always on

### .github/copilot-instructions.md
- GitHub Copilot 専用の常時適用指示ファイル

### AGENTS.md
- 複数の AI Coding Agent が参照する汎用指示ファイル
- ルートに1つ、またはサブディレクトリにネストして適用可能

### CLAUDE.md
- Claude Code 専用の常時適用指示ファイル
- ルートに1つ、またはサブディレクトリにネストして適用可能

### GEMINI.md
- Gemini CLI 専用の常時適用指示ファイル
- ルートに1つ、またはサブディレクトリにネストして適用可能

## 2. Path specific

### .github/instructions/*.instructions.md
- GitHub Copilot 専用のパス固有指示ファイル
- frontmatter の `applyTo` でファイルパターンを指定し、特定のファイルにのみ適用可能

## 3. Custom Agents

### .github/agents/*.agent.md
- GitHub Copilot 専用のカスタムエージェント定義ファイル
- Copilot Chat のエージェントメニューから選択して呼び出し可能
- CLI では `/agent` コマンドで呼び出し可能

## 4. Prompt Files

### .github/prompts/*.prompt.md
- GitHub Copilot 専用の再利用可能なプロンプトファイル
- Copilot Chat で `/` コマンドとして呼び出し可能

## 5. Agent Skills

### .github/skills/*/SKILL.md
- GitHub Copilot 専用のエージェントスキル定義ファイル
- 説明文ベースで自動マッチングされ、スクリプトやテンプレートを含められる

## References

### GitHub Docs

- [Repository custom instructions](https://docs.github.com/en/copilot/customizing-copilot/adding-repository-custom-instructions-for-github-copilot)
- [Customizing Copilot responses](https://docs.github.com/en/copilot/concepts/prompting/response-customization)
- [Custom instructions support](https://docs.github.com/en/copilot/reference/custom-instructions-support)
- [Custom agents](https://docs.github.com/en/copilot/how-tos/use-copilot-agents/coding-agent/create-custom-agents)
- [Agent skills](https://docs.github.com/en/copilot/how-tos/use-copilot-agents/coding-agent/create-skills)
- [Prompt files](https://docs.github.com/en/copilot/tutorials/customization-library/prompt-files/your-first-prompt-file)

### VS Code Docs

- [Custom instructions](https://code.visualstudio.com/docs/copilot/customization/custom-instructions)
- [Prompt files](https://code.visualstudio.com/docs/copilot/customization/prompt-files)
