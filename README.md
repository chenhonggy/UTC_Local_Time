    UTC_Local_Time是一个基于android2.2以上版本的SDK
    拥有UTC时间与本地时间之间相互转换的功能以及UTC时间之间的比较
    通过UTC时间还可以获取不同格式的日期以及星期
    后期还会更新方法的操作方式，使之更加方便
        
####如何开始
#####手动安装
    将Utils文件夹里面的文件复制到您的工程文件下面
        
####开始编码
#####不包含毫秒(yyyy-MM-dd'T'HH:mm:ss'Z')
    工程文件下面的方法都是public static的方法，所以您可以直通过类名来调用方法
    1.通过传入的UTC时间转换成本地时间（UTC时间格式yyyy-MM-dd'T'HH:mm:ss'Z'）
    DateUtils.timestampToDeatil(DateUtils.getUTCCurrentTimestamp())
    2.通过传入的本地时间转成为UTC时间
    DateUtils.getUTCTimestamp(System.currentTimeMillis()+"")
        
#####包含毫秒(yyyy-MM-dd'T'HH:mm:ss.S'Z')
    DateUtils.timestampToLocalDateWithMillisecond(time)
    DateUtils.getUTCTimestampWithMillisecond
    UTC时间格式yyyy-MM-dd'T'HH:mm:ss.S'Z'
        
    
####您还可以
#####不包含毫秒(yyyy-MM-dd'T'HH:mm:ss'Z')
    通过UTC时间获取不同格式的日期与星期
    1.星期
    DateUtils.getLocalweek(time)
    2.yyyy.MM.dd格式的日期
    DateUtils.getLocalYearMonthDay(time)
    3.获取两个UTC时间之间相差的天数
    DateUtils.getLocalDistDatas(utcTimestart,utcTimeend)
        
####更多的方法可以下载浏览，thanks.
<br><br><br>

####最近更新
    版本1.0
    更新内容:UTC与本地时间相互转换以根据UTC时间获取更多本地日期信息
