# 正则表达式

## 3xx
301 永久重定向,告诉客户端以后应从新地址访问.

302 作为HTTP1.0的标准,以前叫做Moved Temporarily ,现在叫Found. 现在使用只是为了兼容性的处理，但是HTTP 1.1 有303 和307作为详细的补充,其实是对302的细化

303：对于POST请求，它表示请求已经被处理，客户端可以接着使用GET方法去请求Location里的URI。

307：对于POST请求，表示请求还没有被处理，客户端应该向Location里的URI重新发起POST请求。