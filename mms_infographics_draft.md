# MMS講義メソッド：インフォグラフィック・ドラフト（Mermaid版）

このファイルは、これまでに言語化したアキさんの「売上10倍の真髄（8ステップメソッド）」を視覚化するためのプロトタイプです。
文字化けを完全に防ぎ、後から文言をいくらでも修正できるように、テキストベースで図を描画できる「Mermaid（マーメイド）」という記法を使用しています。

## 1. カリキュラムの全体像（3つのフェーズと8ステップ）

```mermaid
flowchart TB
    %% スタイル定義
    classDef phase1 fill:#e3f2fd,stroke:#1e88e5,stroke-width:2px,color:#0d47a1
    classDef phase2 fill:#fff3e0,stroke:#fb8c00,stroke-width:2px,color:#e65100
    classDef phase3 fill:#fce4ec,stroke:#e91e63,stroke-width:2px,color:#880e4f
    classDef os fill:#f3e5f5,stroke:#8e24aa,stroke-width:3px,color:#4a148c,stroke-dasharray: 5 5

    subgraph Phase1 [第1フェーズ：器と信頼の構築 BE]
        direction TB
        A["1. 自己の在り方\n(アンカリングで状態を整える)"]:::phase1
        B["2. 価値観の発掘と現場検証\n(ファクトと感情のズレを受容)"]:::phase1
        C["3. 7秒コーチングと承認\n(褒めるのではなく存在を承認)"]:::phase1
        D["4. 弱さの自己開示\n(心理的安全性の担保)"]:::phase1
        A --> B --> C --> D
    end

    subgraph Phase2 [第2フェーズ：対話と目標の統合 DO / TEAM]
        direction TB
        E["5. アサーション\n(相手を傷つけず耳の痛いことを伝える)"]:::phase2
        F["6. 1on1とファシリテーション\n(相手に考えさせ、総論賛成を作る)"]:::phase2
        G["7. 共有ゾーンの形成\n(個人のキャリアと会社の目標の合致)"]:::phase2
        E --> F --> G
    end

    subgraph Phase3 [第3フェーズ：波及と牽引 LEADERSHIP]
        direction TB
        H["8. ストーリーテリング\n(原体験を語り、周囲を巻き込む)"]:::phase3
        I(["圧倒的な成果\n『売上10倍と自走組織』の実現"])
        H --> I
    end

    Phase1 ==>|強固な信頼関係| Phase2
    Phase2 ==>|真のエンゲージメント| Phase3
```

---

## 2. ライフイノベーションマップが貫く「1つの軸 (OS)」

```mermaid
flowchart LR
    %% スタイル定義
    classDef core fill:#ede7f6,stroke:#673ab7,stroke-width:3px,color:#311b92,font-weight:bold
    classDef detail fill:#fafafa,stroke:#9e9e9e,stroke-width:1px

    OS(("圧倒的な成果を生むOS\n『ライフイノベーションマップ』")):::core
    
    Input["【起点：インプット】\n過去の棚卸しと価値観の抽出"]:::detail
    Process["【展開：プロセス】\n揺るぎない自己受容と他者受容"]:::detail
    Output["【終点：アウトプット】\n原体験に基づくストーリーテリング"]:::detail

    OS --> Input
    Input -->|自分が定まるからこそ| Process
    Process -->|相手と通じ合うからこそ| Output
    
    Input -.-> |ステップ1・2へ| Phase1_Link(器の構築)
    Process -.-> |ステップ5・6・7へ| Phase2_Link(対話とファシリテーション)
    Output -.-> |ステップ8へ| Phase3_Link(強烈なリーダーシップ)
```

---

## 3. 「共有ゾーン」形成の詳細メカニズム（ズームアップ）

```mermaid
mindmap
  root((共有ゾーンの<br>形成))
    個人の領域
      キャリアプランの引き出し
      個人の価値観の明確化
      やりたい方向性
    会社の領域
      ミッション・ビジョン
      大切にしている価値観
      組織の目標・売上
    交差点（共有ゾーン）
      1on1での「自発的貢献意欲」
      会議での「総論賛成（目的の合意）」
      不毛な対立の排除
```
