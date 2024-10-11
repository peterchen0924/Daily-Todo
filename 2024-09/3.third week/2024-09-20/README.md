~~錢~~
----
CRR
    機率部分可調整寫法?
    架構assert待改

    1.第一點找方向 算vector 與sink計算座標
    2.轉角??
----
~~s06 google~~

-----
PPSA 圖存座標
1.會不會走回自己 <-先不管
也許記下來，讓封包不要走回到走過的點 misc(path)
把路徑記下來

隨便挑一個點，SPF到
2.假路徑
  分支路徑要倒過來傳
3.紀錄主分支
4.算出src~fake src，再由他們相差的x,y，再推出sink~ fake sink 的x,y座標
5.中間SPF
6.src把設定好的路徑發出，封包說怎麼走，node就照著傳
-----
老師改src發出第一步，目前皆用SPF
pkt_gen
架構assert待改

----


月餅照
防風眼鏡