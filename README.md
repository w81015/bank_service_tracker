
# 銀行服務主題分析

該專案旨在從PTT銀行論壇提取、清理和分析數據。目標是利用LDA（隱含狄利克雷分配）分析揭示流行的主題和見解。該專案分為兩個主要部分：數據收集和數據分析。

## 第一部分：數據收集 (`text_collection.ipynb`)

- **目標**：從PTT銀行論壇爬取數據，重點關注可能提供銀行趨勢、顧客情緒和熱門金融產品有價值的帖子。
- **使用工具**：Python及其庫，如`requests`和`beautifulsoup4`進行網頁爬取。
- **輸出**：一個已清理準備好進一步分析的數據集。

## 第二部分：數據分析 (`lda_analysis.ipynb`)

- **目標**：應用清理技術和LDA分析於收集到的數據上，以識別PTT銀行論壇內的主導主題。
- **使用工具**：Python及其NLP庫，如`ckiptagger`用於中文文本分詞和`gensim`進行LDA建模。
- **輸出**：一組代表PTT銀行論壇主要討論主題的主題集，以及它們各自的詞分布和相關性分數。

## 如何使用

1. **數據收集**：運行`text_collection.ipynb`筆記本收集和預處理來自PTT銀行的數據。
2. **數據分析**：使用清理後的數據，執行`lda_analysis.ipynb`筆記本進行LDA分析，揭示潛在主題。

## 需求

- Python 3.6+
- `pandas`, `jieba`,`requests`, `beautifulsoup4`, `ckiptagger`, `gensim`, `pyLDAvis`。
