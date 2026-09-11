# タスク

## 現在の段階

ゲームは既に遊べる状態にある（`game/underborn_scout8d.html`）。
**2026-09-03 に中断を解除**（DECISIONS 運用・体制）。遺跡単独版の9F hotfix、区画内反転、エンディング、周回まで実装済み。以後は便を Kevin 待ち無しで連続実行し、Kevin は最終決定4つだけを持つ。

## 進行中（担当を AI に付け替え。2026-09-03）

- [x] 女神の出し方：小・ズームなし・その場で吹き出し（Kevin 確定 9-05）
- [x] **Claude**：「女神便」の発注文 `docs/orders/2026-09-05_goddess_v1.md`（9-05）
- [x] **Codex（Sol）**：女神便を実装 → `game/underborn_scout7be.html`。起動確認・完了条件チェック済み（9-06）
- [x] Claude 検品（9-06、HANDOFF「Claude 検品」）：発注文どおり。詩・息止めの教え・儀式は無変更
- [x] Kevin が `scout7be` を見た（9-06）：吹き出しが顔にかぶる／突然出て即消える → hotfix へ
- [x] **Codex（Sol）**：`docs/orders/2026-09-06_goddess-hotfix_v1.md` を実装 → `game/underborn_scout7bf.html`。ランダム配置10例・手動／自動送り・森の二行表示をブラウザ確認（9-06）
- [x] **Codex（Sol）**：`docs/orders/2026-09-06_goddess_v2.md` を実装 → `game/underborn_scout7bg.html`。開始・拒否4段・初進化・森をブラウザ確認（9-06）
- [x] Claude：第7B-b便の発注文 `docs/orders/2026-09-06_7B-b_v1.md`（9-06）
- [x] Sol-R：7B-b v1 をレビュー、9点指摘 → Claude が v2 に反映（9-06）
- [x] **Codex（Sol）**：`docs/orders/2026-09-06_7B-b_v2.md` を実装 → `game/underborn_scout7bh.html`。クリア記録・5土地・孵化・ミニマップ・息吹・持ち越し6件をブラウザ確認（9-06）
- [x] **Codex**：7B-b を実装し、正典を次の世代へ。HANDOFF 更新。実装前に発注文とコードを照合した（9-06）
- [x] **Codex（Sol）**：初回プレイ hotfix を `game/underborn_scout7h.html` として実装。授与前のハーケン、女神の二択入力、暗闇上の穴を修正（9-09）
- [x] **Codex（Sol）**：遺跡16階便を `game/underborn_scout8a.html` として実装。4区画、休憩所、9F・13F進化、保存復帰を反映（9-09）
- [x] **Codex（Sol）**：エンディング便を `game/underborn_scout8b.html` として実装。本番を遺跡だけにし、詩・女神・初変身・住民列・周回と足音を接続（9-10）
- [x] **Codex（Sol）**：`docs/orders/2026-09-10_mirror-floors_v2.md` を `game/underborn_scout8c.html` へ実装。地図・祭壇・巡回点・開始位置の4反転と保存版 `layout:2` を反映（9-10）
- [x] **Astra（別タスク、Kevin が起動）**：遺跡1〜8Fと9F再挑戦まで通し、操作環境の制約により45分で中断。観察4点をhotfixへ渡した（9-10）
- [x] **Codex（Sol）**：`docs/orders/2026-09-10_ninth-floor-hotfix_v1.md` を `game/underborn_scout8d.html` へ実装。開始直後の安全、儀式のラン内1回化、穴カメラ、大広間4配置を反映（9-11）
- [ ] **Codex（プレイ検品）**：息止め移動比率0〜1／捜索2秒／狭通路・行き止まり・複数敵の3点を実プレイし、不自然な点を HANDOFF「実装側の感触」に書く。既定値のまま通るなら暫定行を書かない
- [ ] **Claude**：7B-b3 の検品（diff 読み）。断面図の表示契機は HANDOFF の答え（`drawCrossSection` の呼び出しが無い）を確認して閉じる
- [x] **Claude**：第7C便の発注文を書く（支点一式、v2レビュー反映済み）（9-06）
- [x] **Codex（Sol）**：第7C便を `game/underborn_scout7c.html` として実装。支点設置・保存・ハート0復帰・「つづきから」をブラウザ確認（9-06）
- [x] **Codex（Sol）**：ハーケン便を `game/underborn_scout7d.html` として実装。名称・打つ演出・火が絶える演出・初回授与をブラウザ確認（9-07）
- [x] **Codex（Sol）**：昇階・住民便を `game/underborn_scout7e.html` として実装。初登場台詞・解放・通常昇階・節目カード・地上と森の住民列を反映（9-07）
- [x] **Codex（Sol）**：点火無料便を `game/underborn_scout7f.html` として実装。自己点火のハート消費だけを外し、住民接触と種火連鎖をブラウザ確認（9-08）
- [x] **Codex（Sol）**：穴とハーケンの絵便を `game/underborn_scout7g.html` として実装。通常階の手動昇階、安全状態、縄つきハーケンの授与・HUD・床表示をブラウザ確認（9-08）
- [ ] **Codex**：一般配布用に `DEV_DEFAULT=false` へ戻し、DEV UI が出ないことを確認

## 次に行うこと（暫定行で進める。Kevin は却下だけ）

- [x] Kevin が遺跡16階を通常操作で1周し、「全体的にこんな感じでいいのかも」と確認（9-11）。正確な所要時間と数値評価は未記録
- [ ] Kevinの通し所感3点（エンディングが急／休憩所でできること／スコアの要否）を整理する
- [x] 支点の本数を暫定5本で実装し、開発パネルで3〜5本を試せるようにした（9-06）
- [x] ハートの階またぎと支点復帰時のハート数を既定値（最低3／刺した時点）で実装した（9-06）
- [x] 森のコアの呼称＝息吹で実装した（呼称の最終裁可は未了）

## Kevin の最終決定（AI は草稿まで。採否は Kevin）

- [x] 女神のキャラデザ（Kevin 確定 9-05：`docs/design/goddess-final.png`。DECISIONS 09-05 決定版）
- [ ] 完成の宣言（第一段＝遺跡 MVP）
- [ ] 公開・提出の可否（10月の評価提出物を含む）
- [ ] 提出直前のバランス数値の確定
- [ ] エンディングの詩の最終稿（**草稿は Claude が書く**。森の解放詩の後に置く1篇）とロゴ・キービジュアルの最終判定
- [ ] 女神 v2 の問い・拒否・回想台詞の最終稿（現在は Kevin 案＋Claude 草稿の暫定文）

## 保留

- [x] 2周目は「旅の果て」→周回ダイヤル→遺跡1Fへ戻り、真の姿を解禁する（9-10）
- [ ] 10月の評価提出物の範囲を決める。評価用に階数を落とした分岐を作るか
- [ ] 一枚絵のパイプライン検証（GPT生成→ドット化）
- [ ] ドット絵師・サウンドの募集
- [ ] マップ描画の改善（見た目便として文面作成済み）
- [ ] 旧本線 `dungeon_born_evolution.html` の扱い（8/3時点で停止中）

## 完了

- [x] GitHubリポジトリを作成し、AI共同作業用の基本資料を用意する
- [x] CodexからGitHubリポジトリを参照できることを確認する
- [x] Claudeの既存会話をリポジトリの資料へ移行する
- [x] 第6便までの納品と検品
- [x] 各土地の詩4篇（砂漠・火山・沼・森）を確定する
- [x] 詩の語り手構造（女神／土地の二声）を決める
- [x] 支点の基本設計を決める
- [x] 階数と進化の割合を決める
- [x] 第7便の発注文を書き、レビューを通す（7Aとして分割・確定）
- [x] 第7A便を `game/underborn_scout7a.html` として実装する
- [x] 7Aの構文・通常起動・開発用UI・全土地最上階のブラウザ確認を行う
- [x] 第7A-hotfix便を `game/underborn_scout7ah.html` として実装する
- [x] URL編集なしのデバッグ永続化、無敵、段階指定、敵ゼロを追加する
- [x] 特殊階を進行率25%以降へ後送し、副題削除とタイトル演出スキップを反映する
- [x] 17→18階の実遷移で、進化儀式→暗転→初進化詩の単独表示を確認する
- [x] 第7B-a便を `game/underborn_scout7b.html` として実装する
- [x] シネマティック中の検証パネル、折りたたみ、階数表示、ポーズ、DEV三状態を実装する
- [x] 第7B-b1便を `game/underborn_scout7bb.html` として実装する
- [x] 息止め中の目だけ表現、解除時の小さな膨らみ、息止め秒数・CT調整、光初期値を反映する
- [x] 第7B-b2便を `game/underborn_scout7bc.html` として実装する
- [x] 息止め中の通常移動比率0〜1、マス単位の速度切替、完全停止中のコア固有能力維持を反映する
- [x] 第7B-b3便を `game/underborn_scout7bd.html` として実装する
- [x] 見失い追跡・周辺捜索・巡回復帰、息止め中のマスター座標回避、炎上3秒停止を反映する
- [x] 女神便を `game/underborn_scout7be.html` として実装する
- [x] 新規開始のスポット→女神、進化後の新階→女神、森の解放詩→変身前詩、台詞スキップをブラウザで確認する
- [x] 女神便 hotfix を `game/underborn_scout7bf.html` として実装し、吹き出しの重なり・登退場・一行送りを修正する
- [x] 女神便 v2 を `game/underborn_scout7bg.html` として実装し、「声が先、姿はあと」・選択・拒否記憶へ組み直す
- [x] 第7B-b便を `game/underborn_scout7bh.html` として実装し、クリア保存・地上演出・孵化・ミニマップ・息吹と持ち越し6件を反映する
- [x] 第7C便を `game/underborn_scout7c.html` として実装し、支点設置・保存・復帰・タイトル再開を反映する
- [x] ハーケン便を `game/underborn_scout7d.html` として実装し、名称・打つ演出・火が絶える演出・初回授与を反映する
- [x] 昇階・住民便を `game/underborn_scout7e.html` として実装し、解放住民の記録と列、階を上がる演出を反映する
- [x] 点火無料便を `game/underborn_scout7f.html` として実装し、自己点火を無料にする
- [x] 穴とハーケンの絵便を `game/underborn_scout7g.html` として実装し、光の穴への手動進入と縄つきハーケンの共通表示を反映する
- [x] 初回プレイ hotfix を `game/underborn_scout7h.html` として実装する
- [x] 遺跡16階便を `game/underborn_scout8a.html` として実装する
- [x] エンディング便を `game/underborn_scout8b.html` として実装する
- [x] 区画内反転便を `game/underborn_scout8c.html` として実装する
- [x] 9F hotfix を `game/underborn_scout8d.html` として実装する

## 今回は行わないこと

- 一般配布用の `DEV_DEFAULT=false` 戻し、遺跡16階の長い通しプレイ、他4土地・覚醒コア4種の本番再表示、バランス数値の確定
- `game/underborn_scout6.html` の内容変更（比較用に保存）

- [x] 大広間（13〜16F）の左右反転階に `wideFloor(1)` の別祭壇配置を使い、4階すべての祭壇座標を変える（9F hotfixへ同梱、9-11）

## 見た目（2026-09-10 Kevin 指定。完成＝売りに出せる一歩手前）
- [ ] 様式表（色数・ドットの大きさ・線・光）を1枚決める（Claude 案 → Kevin）
- [ ] 床と壁のタイル
- [ ] 祭壇と、点火したときのエフェクト
- [ ] 住民6種（人でない姿）
- [ ] ベイビーの各姿（卵・ベイビー・チャイルド・ロード・真の姿）
- [ ] HUD・タイトル画面・ロゴ
- [ ] 休憩所・地上の景色
- [ ] BGM（買う／作るを決める）
