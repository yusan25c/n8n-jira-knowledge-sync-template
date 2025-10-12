# 02_Jira_Knowledge-Sync-Pinecone-Indexing
完了済みJiraチケット情報をPineconeに登録するワークフロー（n8n）

## Quickstart
- n8nのWorkflow画面右上「…」→ **Import from file** → `Jira_Knowledge-Sync-Pinecone-Indexing.json` をインポート
- ノードの「!」が消えるまで **認証** を設定（**Jira / OpenAI / Pinecone**）
- 画面下部の **Execute workflow** で実行

## 必要要件
- n8n（Self-Hosted / Cloud いずれも可）
- APIキー：**Jira**（Base URL / Email / API Token）、**OpenAI**（API Key / Model）、**Pinecone**（API Key / Index / Project）

## セットアップ（任意の詳細）
- n8nインストール（Docker Compose 例）：公式ドキュメント参照  
  https://docs.n8n.io/hosting/installation/server-setups/docker-compose/#5-create-local-files-directory

## 使い方
1. ワークフローを開く → ノードの警告「!」をすべて解消  
   - **Jira** 認証は対象サイトの **Base URL** と **Email+API Token** を設定  
2. **Execute workflow** でテスト→ 完了済みJiraチケット情報がPineconeに 登録されます

## その他

改善提案やバグ報告は、GitHubのIssuesまたはPull Requestでお願いします。
