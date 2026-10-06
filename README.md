# ずんだWebゲームズ (araipanda/web_game)

ブラウザでサクッと遊べるPure HTML5/JavaScriptのミニゲーム集です。
GitHub Pagesで静的ホスティングされ、スマホ・PCのどちらでもインストール不要で楽しめます。

## 🎮 公開URL
- **ポータル（ゲーム一覧）**: [https://araipanda.github.io/web_game/](https://araipanda.github.io/web_game/)
- **飛び立て！ずんだもん**: [https://araipanda.github.io/web_game/flappy-zunda.html](https://araipanda.github.io/web_game/flappy-zunda.html)
- **英単語ラッシュ**: [https://araipanda.github.io/web_game/word-rush.html](https://araipanda.github.io/web_game/word-rush.html)

---

## 🕹️ 収録ゲーム一覧

### 1. 飛び立て！ずんだもん（Flappy Zunda）
- **ファイル**: `flappy-zunda.html`
- **概要**: 画面タップでポヨンと跳ねて、枝豆サヤをくぐり抜けるエンドレスアクションゲーム。
- **特徴**:
  - 外部アセットゼロ（HTML5 Canvas + Web Audio APIによるプロシージャル描画・音源合成）
  - スマホ片手操作に特化（`touch-action: manipulation`によるダブルタップ拡大誤爆防止）
  - 可変リフレッシュレート対応（`deltaTime`正規化により60Hz/90Hz/120Hzスマホで速度一定）
  - Safari 16未満対応（`roundRect`ポリフィル搭載）
  - BGM/SEミュート切替対応（設定はローカルストレージ保存）

### 2. 英単語ラッシュ（Word Rush）
- **ファイル**: `word-rush.html`（`word_rush.html`）
- **概要**: 60秒間でどれだけ英単語を回答できるかを競う超高速3択タイムアタックゲーム。
- **特徴**:
  - 外部アセットゼロ（HTML1枚完結・CSSアニメーション＋Web Audio APIによるシンセ効果音）
  - 3難易度（Easy/Normal/Hard）× 各75語 ＝ 計225語収録
  - 誤答選択肢の動的ランダムサンプリング（同義語・重複選択肢の排除ガード搭載）
  - 周回プレイ時の連続重複出題防止ガード（20万回シミュレーション検証済み）
  - コンボ＆スピードボーナス、FEVERモード、localStorageハイスコア記録
  - 回答後の高速遷移（130ms/250ms）と誤連打防止ディレイガード搭載

---

## ⚙️ GitHub Pagesの有効化手順
1. 本リポジトリの **Settings** タブを開く
2. 左メニューの **Pages** を選択
3. **Build and deployment** > **Source**: `Deploy from a branch`
4. **Branch**: `main` / `/ (root)` を選択して **Save** を押す
5. 数分後、上記URLでゲームが公開されます。
