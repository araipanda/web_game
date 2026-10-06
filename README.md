# ずんだWebゲームズ (araipanda/web_game)

ブラウザでサクッと遊べるPure HTML5/JavaScriptのミニゲーム集です。
GitHub Pagesで静的ホスティングされ、スマホ・PCのどちらでもインストール不要で楽しめます。

## 🎮 公開URL
- **ポータル（ゲーム一覧）**: [https://araipanda.github.io/web_game/](https://araipanda.github.io/web_game/)
- **飛び立て！ずんだもん**: [https://araipanda.github.io/web_game/flappy-zunda.html](https://araipanda.github.io/web_game/flappy-zunda.html)

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

---

## ⚙️ GitHub Pagesの有効化手順
1. 本リポジトリの **Settings** タブを開く
2. 左メニューの **Pages** を選択
3. **Build and deployment** > **Source**: `Deploy from a branch`
4. **Branch**: `main` / `/ (root)` を選択して **Save** を押す
5. 数分後、上記URLでゲームが公開されます。
