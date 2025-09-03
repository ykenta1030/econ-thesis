## main DiD
## scenario one DML outcome(順序尺度だが、間隔尺度として・・・）
## scenario two DML outcome(ダミー変数として）

# 経済学修士研究（因果推論 × データ分析）
テレビCMが購買意欲に与える影響を、計量経済学的手法を用いて分析したプロジェクトです。

## 背景・目的
- 広告効果測定の重要性が高まる中、テレビCMが消費者行動に与える影響を実証的に検証しました。
- 第一目的 : DMLを用いて、CATEを導出し、何らかの示唆を出す

## 使用データ
- 野村マーケティング（コンペに出場）から提供
- 視聴ログ、CM出稿データ、アンケート調査データなど

## 手法・技術スタック
- Python (pandas, scikit-learn, LightGBM, econml, statsmodels)
- 因果推論手法
  - Difference-in-Differences (DID)
  - Double Machine Learning (DML)
  - Propensity Score Weighting 
- 可視化: matplotlib, seaborn
- バージョン管理: Git, GitHub

## 分析フロー(全体）
1. データ前処理
   - 欠損値補完、カテゴリ変数のエンコーディング
2. 傾向スコア推定（LightGBM）
3. マッチング & 重み付けによる共変量バランス調整
4. 因果効果推定（DID, DML）
5. 可視化・解釈

## 結果
- CM視聴は購買意欲など条件付けなしでは効果がない

## 学び・今後の展望
- 因果推論の理論と実務的な分析の橋渡しを経験
- 現時点は途中なので、これから新たしい仮説を出し、分析を増やす予定
- 今後は、オンライン広告やEC分野への応用も探求予定

## リポジトリ構成
- `notebooks/` : 分析用 Google colab
- `README.md` : 本ファイル
