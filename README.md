# **House Prices - Advanced Regression Techniques**  
## ◇ プロジェクト概要
Kaggleコンペティション「**House Prices - Advanced Regression Techniques**」のデータを用いて、  
住宅価格の予測モデルの構築に取り組んだプロジェクトです。  
  
Baselineモデルの作成を起点に、  
交差検証・特徴量の把握・モデル選定・スケーリングによる分布調整・ハイパーパラメータの最適化などを通じて、    
**予測精度の向上とモデルの解釈性の向上**を目指しました。  
  
モデルの改善の各ステップを通じて、最終的に **Public Score 0.12329** を記録。  
全参加者4134名中406位となり、 **上位10％以内にランクイン** することができました。  
ベースラインから段階的な改善を行い、  
**可視化・変換処理・モデル最適化の工程が実際の精度向上に直結した**ことを確認できた取り組みです。  

コンペティションページ  
=> [House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)  

## ◇ 実施内容
- Baselineモデルの構築 (RandomForestRegressor)
- KFoldによる交差検証とモデル評価
- 単一モデルにおけるアンサンブル的学習
- EDAによるデータ分布・外れ値の確認と処理
- モデル選定: LightGBMRegressor・CatBoostRegressor の適用
- ハイパーパラメータ最適化・比較
- Kaggle提出スコア (Public LB)  
  - Baseline (RandomForestRegressor): **0.14767**  
  - MainModel (LightGBMRegressor): **0.12836**  
  - MainModel (CatBoostRegressor): **0.12329** (最良スコア)  

## ◇ ファイル構成
- House-Prices_Baseline.ipynb: 基準となるベースラインモデル
- House-Prices_MainModel.ipynb: ベースモデルを基準としたメインモデル
- README.md: 本ファイル。プロジェクトの概要や構成を記載

## ◇ ノートブック実行リンク
- House-Prices_Baseline.ipynb (初期ベースラインモデル)  
  => [Google Colabで開く](https://colab.research.google.com/drive/1gLcwyxNlV9y-dIHifx6WD5d3Vhdb3pbx?usp=drive_link)   
- House-Prices_MainModel.ipynb (メインモデル)  
  => [Google Colabで開く](https://colab.research.google.com/drive/1NmvA6oncm1ba823WDYHboDJDxjpCIEhm?usp=drive_link)

> ※ 実行には 'kaggle.json' のアップロードが必要です。

## ◇ 学び・得られたこと
- **段階的なアプローチ** によって、精度を着実に向上させる力の体得。  
  => ベースラインからスタートし、モデル変更・スケーリング・外れ値処理と、改善を積み重ねたことで、  
  　最終的に **Public LB 上位10% (4134人中406位)** にランクイン
    
- スコアやデータを客観的に捉え、適切な判断に基づくモデル選定。  
  => LightGBM と CatBoostの比較において、カテゴリ型の扱いやデフォルト性能の違いを理解し、  
  　**問題に合ったモデル選択と適用の力** を養えました。  
    
- 可視化による分析を通じて、外れ値や分布の偏りの発見・処理。  
  => EDAを通じて得られた示唆から、スケーリングを柔軟に導入し、  
  　**データの形状に合わせた前処理の重要性** を体感しました。
  
---
最後までご覧いただき、ありがとうございました。  
本プロジェクトを通じて得た学びや気づきが、今後のさらなる成長と挑戦につながるよう、  
引き続き、取り組んでまいります。  