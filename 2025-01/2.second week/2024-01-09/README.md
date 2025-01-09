    1.ppt 畫圖
    2.ppt 列出大綱順序?
    3.整理圖


    random皆各為幾步???
        PW:(short:2,3,…,0.5×Δss ; long:2+Δss,…,1.5×Δss )
        SRR_R:沒寫，圖片表示2
        PPSA:沒寫，設定? 2或5

    attacker 多久回退??
        -Attacker_moving_delayUS = 100
            # if distance=200m, speed=72km/hr=7.2*10^4m/3.6x10^6ms=2*10^-2m/ms=20m/s=> 200m/(20m/s)=10s        
        -Attacker_waitPkt_timeoutUS = 100 # the time the attacker wait to check if it detect any pkt transmission signal when staying at a node
        -Attacker_patientWait_maxRetry = 5 # number of max retry if the attacker did not receive any pkt when wait for detecting pkt transimmision signal

    討論:
        1.PPSA　attacker多久?
        2.一定會被誘導進去(因為時間差?) fakeSrc 改發送頻率?
        3.數據?

        #移動到哪裡
        #知道去哪裡
        40hops
        