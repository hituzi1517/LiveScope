# LiveScope
YouTube Live の公開同時視聴者数を YouTube Data API v3 から定期取得し、ブラウザ内に保存・グラフ化する静的PWAです。

## GitHub Pages
1. このフォルダの中身をリポジトリ直下へアップロード。
2. Settings → Pages → Deploy from a branch → `main` / `(root)`。
3. Google Cloud Console で YouTube Data API v3 を有効化し API キーを作成。
4. APIキーには Websites / HTTP referrers の制限と、YouTube Data API v3 の API 制限を設定することを推奨。

## 注意
iOS/Safari/PWAはバックグラウンドでJavaScriptの実行が止まることがあり、その間の同接は取得できません。終了済みライブの過去同接はYouTube Data APIから復元できません。
