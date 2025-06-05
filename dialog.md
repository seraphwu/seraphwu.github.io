```mermaid
graph LR
    subgraph AI應用領域
        direction LR
        App1[智能檢索]
        App2[問答系統]
        App3[推薦系統]
        App4[數據集成]
        App5[臨床決策支持]
        App6[機器人場景理解]
    end

    subgraph AI核心能力
        direction TB
        NLU[自然語言理解]
        KR[知識推理]
        ML[機器學習/深度學習]
    end

    subgraph 知識組織與表示工具
        direction TB
        Thes[索引典 Thesaurus]
        Onto[本體論 Ontology]
        KG[知識圖譜 Knowledge Graph]
        SW[語義網 Semantic Web (框架/原則)]
    end

    Thes -->|提供詞彙控制| NLU
    Onto -->|定義語義模型| NLU
    Onto -->|提供形式化知識| KR
    KG -->|提供結構化事實| KR
    KG -->|作為訓練數據/特徵| ML
    SW -->|提供標準和互操作性| Onto
    SW -->|提供標準和互操作性| KG

    NLU --> App1
    NLU --> App2
    NLU --> App6
    KR --> App2
    KR --> App4
    KR --> App5
    KR --> App6
    ML --> App1
    ML --> App3
    ML --> App5

    style App1 fill:#lightgreen,stroke:#333,stroke-width:2px
    style App2 fill:#lightgreen,stroke:#333,stroke-width:2px
    style App3 fill:#lightgreen,stroke:#333,stroke-width:2px
    style App4 fill:#lightgreen,stroke:#333,stroke-width:2px
    style App5 fill:#lightgreen,stroke:#333,stroke-width:2px
    style App6 fill:#lightgreen,stroke:#333,stroke-width:2px

    style NLU fill:#lightblue,stroke:#333,stroke-width:2px
    style KR fill:#lightblue,stroke:#333,stroke-width:2px
    style ML fill:#lightblue,stroke:#333,stroke-width:2px

    style Thes fill:#orange,stroke:#333,stroke-width:2px
    style Onto fill:#orange,stroke:#333,stroke-width:2px
    style KG fill:#orange,stroke:#333,stroke-width:2px
    style SW fill:#orange,stroke:#333,stroke-width:2px
```
