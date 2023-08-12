# 內存對齊
**除了C/C++以外，只要可以跨平台的編程語言都需要做內存對齊，包含Java, Python。**
+ 為甚麼會有[內存對齊](https://github.com/youngyangyang04/leetcode-master/blob/master/problems/%E5%89%8D%E5%BA%8F/%E5%88%B7%E4%BA%86%E8%BF%99%E4%B9%88%E5%A4%9A%E9%A2%98%EF%BC%8C%E4%BD%A0%E4%BA%86%E8%A7%A3%E8%87%AA%E5%B7%B1%E4%BB%A3%E7%A0%81%E7%9A%84%E5%86%85%E5%AD%98%E6%B6%88%E8%80%97%E4%B9%88%EF%BC%9F.md)?
    1. 平台原因：不是所有的硬件平台都能訪問任意內存地址上的任意數據，某些硬件平台只能在某些地址處取某些特定類型的數據，否則拋出硬件異常。為了同一個程序可以在多平台運行，需要內存對齊。

    2. 硬件原因：經過內存對齊後，CPU訪問內存的速度大大提升。
+ 內存對齊浪費內存資源?
    是。但實際上來說，計算機內存資源一般都是充足的，我們更希望提高執行速度。
    
**編譯器一般都會做內存對齊的優化操作，也就是當考慮程式真正占用的內存大小時，也需要認識到內存對齊的影響。**