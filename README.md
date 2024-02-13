# scRNAseq_handson_2023

Python を用いたシングルセル RNA-seq 解析。

https://github.com/genome-sci/python_bioinfo_2023
2-3の続き。

1. Cell typeのアノテーション（マニュアル、自動）
2. リファレンスアトラスとの統合解析
3. RNA Velocity

### 手順

```
# ソースコード取得
git clone https://github.com/khigashi1987/scRNAseq_handson_2023.git

cd scRNAseq_handson_2023/

# データファイル取得
wget http://palaeo.nig.ac.jp/Resources/PAGSTutorial2023/retinal.h5ad
（あるいは上記リンクにアクセスしてファイルをダウンロード）
mv retinal.h5ad ./data
（ダウンロードしたretinal.h5adは、scRNAseq_handson_2023/data内に配置してください）

# jupyter notebook起動
jupyter notebook
```

### Dockerによる実行
https://github.com/genome-sci/python_bioinfo_2023 で構築した pags:2023 イメージで実行可能。
