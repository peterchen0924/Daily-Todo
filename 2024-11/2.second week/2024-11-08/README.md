~~1.fakePath 轉 id~~
~~srcId 正確~~
~~目前fakesrc一直發?~~
commRange


2.methodCode改要做的人才寫
-context 接setting
-source 第一個如何發封包
-relay node

3.論文
能源 收幾個&收幾個
total:加起來

4.attacker 手動調整參數，多跑幾次圖

-------
~~目前fakesrc一直發? true、false問題?~~
~~context event少了幾行?~~

寫attacker
停多久? maybe等兩步同樣的 handleEvent_pktIn
沒有收到其他人，only fakeSrc
如何走回去? 紀錄自己走過的路? 不會走回原本的路
在一定時間內會收到兩個封包，丟個骰子往一個方向走，紀錄此點為叉路，不對再往回走
(法一記叉路，法二記錄所有走過的路並存成candidates)
*法二佳，其他人也可避免走重複的路
走回去要走多少步?
怎麼知道Src & fakeSrc? 假設直接知道 (self.isFakeSource) self.isSourceNode 不用測
eg.改lastVisited=G
四面八方送封包(只是看到不是自己)
//聽到有個聲音，直到走到現場聽到一個聲音，
//怎麼知道旁邊沒人，因為沒聽到其他人的聲音，只聽到fs發出的聲音

