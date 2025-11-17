# 🐍 Python仮想環境（venv）操作メモ - Windows環境

このメモは、Pythonプロジェクトのローカル環境構築に必要な主要コマンドを記載しています。
`<ENV_NAME>` は任意の仮想環境名に置き換えて使用してください。（例：`.venv`）

## 1. 仮想環境の基本的な作成と操作

| 項目 | Windows (Command Prompt/PowerShell) |
| :--- | :--- |
| **仮想環境作成** | `python -m venv <ENV_NAME>` |
| **アクティベート** | `.\<ENV_NAME>\Scripts\activate` |
| **非アクティベート** | `deactivate` |
| **（補足）環境確認** | `where python` |

**推奨事項:** `<ENV_NAME>` には慣習的に `venv` を使用することを推奨します。

---

## 2. VS Codeでの利用（推奨される効率的な方法）

VS Codeでは、ターミナルで手動アクティベートを行う代わりに、インタープリタを設定することが最もエラーが少なく効率的です。

1.  上記コマンドで仮想環境を作成（例: `python -m venv venv`）。
2.  **VS Codeを起動**し、プロジェクトフォルダを開く。
3.  `Ctrl+Shift+P` でコマンドパレットを開き、「**Python: Select Interpreter**」を検索・選択。
4.  作成した仮想環境（`<ENV_NAME>` フォルダ内の `python.exe`）を選択する。

**利点:** VS Codeの統合ターミナルやデバッグ実行が自動的に仮想環境を使用するため、手動実行の手間が省略されます。
