
1.PPSA
2.500*500
 50
3.PPT
4.影片

-------

~~PPSA 加好random~~



~~relay 沒轉傳??~~

~~pchome~~

小問題:
    srr_r != totalpktSent?

說法:(待整)
    intercept收得更多的話，有越多的機率(線索)被追蹤到

    乘上有效率

    送一次 可能=收10次

    ourMethod d放大
    根據SPF，長的就長，短的就短(動態調整)
    再乘上倍數~
    1.多餘路徑的比例 = 多少繞的路徑(繞路的情形)
    2.所有的花費 flooding、分支
    3.相等代表沒有額外，>代表額外路徑的比例是多少?

    為什麼不能只看capture? 舉例
    四角放煙火

    1342 1 盡量讓attacker遠離
    寫or講法memo:attacker先看一個，看兩個，看三個仍有2/3機率

紀錄:
    random皆各為幾步???


    attacker 多久回退??
        -Attacker_moving_delayUS = 100
            # if distance=200m, speed=72km/hr=7.2*10^4m/3.6x10^6ms=2*10^-2m/ms=20m/s=> 200m/(20m/s)=10s        
        -Attacker_waitPkt_timeoutUS = 100 # the time the attacker wait to check if it detect any pkt transmission signal when staying at a node
        -Attacker_patientWait_maxRetry = 5 # number of max retry if the attacker did not receive any pkt when wait for detecting pkt transimmision signal

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
