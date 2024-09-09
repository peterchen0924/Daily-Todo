alex




344 random_walk需走與sink反向
~~ 封包需先default~~
順逆 & section不是記在封包? maybe
    1.全域變數 //
    2.packet id 0 順、逆
!!354 第一個random_walk_k=0的人才能選section，並記錄選到的section、方向、
    最後選到的角度至封包//需一個變數來記錄這是第一個人，並存進封包
    其餘的看角度到達沒，還沒就繼續傳
        366 too_close
        #381 寫回封包
        #386 隨機選一個度數
        405 計算向量，並call function


1. testing 全域變數 tuple(正section,副section,順逆)
往外，所以越大越好
2. ~~376 too_close~~
3. 431 selected_angle vector? 需儲存start的座標
4. 439 angle繞圈 
random_walk_k 二階換三階 #角度到達，設random_walk為-1，表示進入第三階段or一個全域變數
5.random_walk 反向傳

老師改src發出第一步，目前皆用SPF
pkt_gen