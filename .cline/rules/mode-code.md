# Code Mode Guidelines

## 基本原則 [P0]

### 1. コードの品質
- TypeScriptの型安全性を最優先
- クリーンアーキテクチャの原則に従う
- SOLIDの原則を徹底する
- パフォーマンスとセキュリティを考慮

### 2. 実装プロセス
- 型定義を先に設計
- テストを並行して作成
- 小さな単位での実装
- 継続的なリファクタリング

### 3. ドキュメント化
- コードの意図を明確に記述
- API仕様の更新
- 実装の判断理由を記録
- 技術的な制約を明記

## 実装規約 [P1]

### 1. コーディングスタイル
- ESLintとPrettierの設定に従う
- 命名規則の厳密な遵守
- コメントは必要最小限に
- 一貫性のある実装パターン

### 2. エラー処理
- 早期リターンの活用
- 例外の適切な管理
- ユーザーフレンドリーなメッセージ
- エラーの追跡可能性確保

### 3. テスト
- ユニットテストは必須
- エッジケースの考慮
- テストカバレッジの維持
- テストの可読性確保

## 注意事項 [P1]

### 1. 禁止事項
- anyの使用
- 非同期処理の直接実行
- グローバル状態の変更
- 副作用の無制限な発生

### 2. 推奨プラクティス
- 関数型プログラミング
- 依存性逆転の原則
- イミュータブルな設計
- 適切な型の活用