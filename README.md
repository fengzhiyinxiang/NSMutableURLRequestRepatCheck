# NSMutableURLRequestRepeatCheck
1. aop方式，debug模式下启用。
2. 基于HttpBody判断相同请求，如果在预先设置的时间内多次发送相同值的HttpBody，则在控制台打印请求SameHTTPBody字符串和HTTPBody转换后的NSDictionary。
3. 重复请求判定时间和判断时请求发送最大字节数可以使用类方法修改。
4. 运行后一段时间后，在控制台搜索SameHTTPBody则可以定位到HttpBody重复发送的情况。
5. 更优化的用法可能是弹出一个提示，或者埋点等。
