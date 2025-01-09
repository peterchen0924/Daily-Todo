1.論文
2.跑一跑
baseNode distanceToNodeById (先不管，可整理)


------
hop count來決定
近 往外選
遠 往內選
----
紀錄:
-實驗參數:
    1.方法
    2.圖長寬大小
    3.實驗最長時間maxTime
    4.src、sink位置
    srcPktGenPeriod = 50

-結果
    1.抓到的時間=lifetime
        -simulation done
        -沒抓到
    2.totalpktSent
    3.totalpktRecv
    4.sink 接到多少封包
    5.attacker 接到多少封包
    6.sink收到，到達的hop_count=latency
    7.TransDelay


比較
-1.抓到的時間 = lifetime，simulation done
-2.Capture ratio 被攻擊者抓到的次數 / 實驗次數
-3.latency = 到達的hop_count (sink接到source封包的時間)
4.Transmission_delay = sendingTime - recvTime (可放可不放，可由3來推)
-5.Intercept rate: attacker收到多少不同的封包/src發多少封包
-6.energy使用多少 = nPktSent*engPerPktSent + nPktRecv*engPerPktRecv



可做多輪再平均
最後算:
    latency，最後要將多次平均*
    energy使用多少 = nPktSent*engPerPktSent + nPktRecv*engPerPktRecv
    沒抓到可算捕獲率*

-----
基礎版SPF可算進比較對象!
----
~~12月椅子~~

