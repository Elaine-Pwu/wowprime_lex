# wowprime_lex
2024黑客松競賽-我要王品禮券組
Amazon Lex 實作方式
1.	建立一個Amazon Lex  Bot - WowPrimeChatbot1
2.	可以選擇兩種不同語言的chatbot模型 （English/Mandarin)
3.	本次主要先實作中文介面的部分，通過建立意圖(intents)以加入觸發的功能，以下是三個主要骨幹功能
a.	Greetingintent- 負責接收使用者的問候，並回答介紹自己的功能
b.	Restaurant_search_ch- 當使用者通過"餐廳"等的資訊進行詢問，chatbot會針對使用者的回答進行分析找到合適的餐廳選擇，並會給予品牌的基本介紹
c.	Foodtypeintent- 當使用者輸入“餐點類型”時，會觸發此功能，針對使用者的回應給出餐廳的建議
4.	在intent中，我們有用到slot，作為輸入類型偵測與對應的橋樑例如：
a.	restaurants-存放王品旗下所有品牌的名稱與縮寫
b.	typeoffood-存放根據王品給的各品牌類型作為基礎的關鍵詞等
