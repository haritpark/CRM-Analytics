# Voice of Customer
## Import Dataset
Wongnai Review dataset contains 300 customer's review

## Import Language Model for universal-sentence-encoder-multilingual
The model details are following:
  - Developed by researchers at Google, 2019
  - Convolutional Neural Net.
  - Covers 16 languages, showing strong performance on cross-lingual retrieval.
  - The input to the module is variable length text in any of the aforementioned languages and the output is a 512 dimensional vector.
  - A larger model with more complicated encoder architecture is available.

## K-Means Clustering
4 Cluster using Elbow method

![image](https://user-images.githubusercontent.com/47063720/147678157-5354aa69-9973-4ba9-8d73-7d033cc65aeb.png)

## Result
Top 10 words for each clusters

![image](https://user-images.githubusercontent.com/47063720/147678234-3404ddc6-6c84-4fb4-ae85-a907427a846b.png)

## Summary
* cluster0 = "ร้านคาเฟ่ ขายกาแฟ ขนม ให้คนมานั่งทำงาน"
* cluster1 = "ร้านอาหารสำหรับครอบครัว เพื่อน"
* cluster2 = "ร้านเครื่องดื่ม ประเภท ชานมไข่มุก ชา นม"
* cluster3 = "ร้านอาหาร รวมทั้งขาย เครื่องดื่ม กาแฟ เป็นร้านที่ดัง ได้รับรีวิวเยอะ"
