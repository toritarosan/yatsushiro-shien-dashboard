# 八代市 災害支援情報ダッシュボード（令和8年熊本地震）

2026年7月28日16時27分発生の「令和8年熊本地震」（八代市は震度6強）について、
八代市民向けの災害支援情報を一枚に集約した静的ダッシュボード。

八代市は**県内最多の死者20人**、**市内全域の断水（県集計約25,300戸／復旧見通し立たず）**、
**都市ガス8,892戸の供給停止**など、今回の地震で最も深刻な被害を受けた自治体の一つ。

- **公開URL**: https://toritarosan.github.io/yatsushiro-shien-dashboard/
- **情報の時点**: 2026-08-22 12:06 JST（各項目に出典と時刻を明記）
- **構成**: `index.html` 1ファイル完結（外部依存なし・ビルド不要）
- **姉妹版**: [宇城市版](https://toritarosan.github.io/uki-shien-dashboard/)（[リポジトリ](https://github.com/toritarosan/uki-shien-dashboard)）

## Claude Codeへの引継ぎ

継続更新する場合は最初に [`CLAUDE.md`](CLAUDE.md) を読んでください。
八代市固有の注意点（水道の所管が2つに分かれている、URLのkiji番号を推測してはいけない等）を記録しています。

## 編集方針（このリポジトリの規律）

1. **出典主義**: 全項目に出典リンクと「いつ時点か」（時刻がわかるものは時刻まで）を付ける。出典を示せない事実は書かない
2. **未確認の明示**: 本文まで確認できなかった情報・公式発表が見つからない事項は「未確認」「準備中」と明示する（「まだ確認できていないこと」セクション）。ねつ造は絶対にしない
3. **一次情報優先**: 市公式 > 県・国公式 > 事業者公式 > 報道の順に優先。報道由来の情報はその旨を出典に明記
4. **時点の明記**: 被害数値は速報値であり時点により異なるため、必ず「◯月◯日 ◯時時点」を併記
5. **URLを推測しない**: 八代市のページURL（kiji番号）は必ず[関連情報ページ](https://www.city.yatsushiro.lg.jp/kiji00326750/index.html)のリンク一覧で実物を確認する

## データソース（主要）

- [八代市 令和8年熊本地震 関連情報](https://www.city.yatsushiro.lg.jp/kiji00326750/index.html) / [緊急情報](https://www.city.yatsushiro.lg.jp/kinkyu.html)
- [熊本県 特設ページ](https://www.pref.kumamoto.jp/soshiki/1/274517.html) / [県災害対策本部資料](https://www.pref.kumamoto.jp/soshiki/222/274487.html)
- [内閣府防災](https://www.bousai.go.jp/updates/r8kumamoto_jishin/index.html) / [厚労省](https://www.mhlw.go.jp/stf/newpage_75017.html) / [国交省](https://www.mlit.go.jp/saigai/saigai_260728.html)
- [八代生活環境事務組合](https://seikatsu.yatsushiro.jp/)（鏡・千丁・東陽・泉の水道）
- [九州ガス](https://www.kyugas.co.jp/r8_kumamoto_info/) / [熊本日日新聞 ライフライン情報](https://kumanichi.com/life2026)

## 完了定義

- [x] 市・県・国・ライフライン・交通・医療・報道・支援団体を横断した初版（2026-08-01時点、358件の調査から構成）
- [x] 全項目に出典リンク＋時点（時刻）を明記
- [x] 未確認事項の明示セクション
- [x] HTMLタグ整合性・アンカーリンク切れなしを機械検証
- [x] 八代市の全URLを市公式のリンク一覧と突き合わせて実在確認
- [ ] GitHub Pages公開・実機（スマホ）表示確認
- [x] 自動巡回ルーティンの設置（1日複数回、GitHub Actions/スケジュール実行で継続稼働中）

## 免責

本ページは公開情報を整理した非公式まとめです。生成AIを用いて作成しています。
内容の正確性・最新性は保証されません。行動の前に必ず各出典（一次情報）を確認してください。

作成: 小金井市 永鳥太郎 ／ 2026-08-01
