# noren-uptime

noren-ai.jp（HP）と analytics.noren-ai.jp（暖簾AI アプリ）の死活監視。

- 15分おきにGitHub Actionsが両URLを確認
- 落ちていたら `outage` ラベルのissueを自動作成（→GitHubからメール通知が届く）
- 回復したらissueを自動クローズ
- 手動テスト: Actions → uptime → Run workflow → force_fail=yes
