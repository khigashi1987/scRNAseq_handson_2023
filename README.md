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
ウェブブラウザで
https://drive.google.com/uc?export=download&id=1ciXMTLSdbkZIRyo8_TZLZjewpGjU9EOB
にアクセスしてファイルをダウンロードする。
（上記リンクから取得できない場合は以下からもダウンロード可能： http://palaeo.nig.ac.jp/Resources/PAGSTutorial2023/retinal.h5ad）
mv retinal.h5ad ./data
（ダウンロードしたretinal.h5adは、scRNAseq_handson_2023/data内に配置してください）

# jupyter notebook起動
jupyter notebook
```

### Dockerによる実行 (amd64のみ)
https://github.com/genome-sci/python_bioinfo_2023 で構築した pags:2023 イメージで実行可能。

```
# 上記手順
git clone https://github.com/khigashi1987/scRNAseq_handson_2023.git
cd scRNAseq_handson_2023/
# ファイルのダウンロードと data への配置
# を実行した後、自分が scRNAseq_handson_2023 にいることを確認して、以下を実行
docker run -it --rm -v $PWD:/python_bioinfo_2023 -p 8888:8888 pags:2023
# ウェブブラウザから http://localhost:8888 を開く
```
