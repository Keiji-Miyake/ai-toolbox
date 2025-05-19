# ai-toolbox

AI支援開発のための設定・プロンプト・instruction管理リポジトリ

## 概要

**ai-toolbox**は、AIコーディングエージェント（GitHub Copilot, Cline, Cursor等）や各種AIツールのための「プロンプト・instruction・設定ファイル」を一元管理するためのリポジトリです。

- 自分が使うAIツールの挙動やルール、プロンプト、instructionを柔軟に管理・拡張できます
- 技術スタックや用途（Web, Python, Go, Rust等）ごとに必要な設定ファイルを選択・カスタマイズ可能
- テンプレートやCLIツールも補助的に提供

## 主な管理内容

- `.github/instructions/`：AIエージェント用のinstruction・コーディング規約
- `.github/prompts/`：AIエージェント用のプロンプトテンプレート
- `.clinerules`, `.clineignore`：Cline用のルール・除外設定
- `.roomodes`：カスタムAIモード定義
- その他、AIツールや技術スタックごとの設定ファイル

## 使い方


### 1. 必要なファイルだけダウンロード

- 利用したいAIツールや技術スタックに応じて、必要なinstructionやプロンプトファイルだけをコピーして使えます
- 例：Copilot用のinstructionだけ使いたい場合は`.github/instructions/copilot-instructions.md`のみ取得


### 2. リポジトリごとcloneしてカスタマイズ

- `git clone https://github.com/yourusername/ai-toolbox.git`
- 自分の開発環境やプロジェクトに合わせて、各種設定・プロンプトを編集


### 3. CLIツール・テンプレートの利用（任意）

- `create-project` CLIなど、AI支援開発に便利なテンプレート生成ツールも同梱
- 必要に応じて`npx create-project myapp`等で雛形を生成


## 特徴・方針

- AIエージェントの挙動・ルール・プロンプトを一元管理
- 技術スタックやAIツールの追加・切り替えも柔軟に対応
- Copilot/Cline/Cursor/Python/Go/Rustなど、今後も拡張予定
- 基本的に自分用だが、他のAIツール利用者にも参考になる構成

## ディレクトリ構成例

```tree
.
├── .clinerules        # Clineのグローバルルール設定
├── .clineignore       # Cline用の除外ファイル設定
├── .github
│   ├── instructions   # AIエージェント用instruction
│   ├── prompts        # AIプロンプトテンプレート
│   └── copilot-instructions.md
├── .roomodes          # カスタムAIモード定義
└── ...（今後拡張）
```

## カスタマイズ例

- `.clinerules`：AIの動作ルールをMarkdownで記述
- `.roomodes`：特定タスク用のAIモードをJSONで定義
- `.github/instructions/`：各AIエージェントごとのinstructionを管理

## 今後の展望

- ClineやCursorへの移行・拡張も検討中
- Python, Go, Rust等のAI支援開発用設定も順次追加予定
- テンプレートやCLIツールも必要に応じてアップデート

## ライセンス

MIT

## お問い合わせ・貢献

- 基本的に自分用ですが、IssueやPR歓迎です。
- 質問・提案はIssueからどうぞ。
