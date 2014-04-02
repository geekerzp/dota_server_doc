通信协议
--------
服务器和客户端使用json进行通信，通信数据进行加密

响应数据格式如下:

    {
      'result': True/False,
      'code': xxx,
      'message': xxx,
      'data': {
        xxx: xxx,
        ...
      }
    }

result:   请求执行成功或数据正确。
code:     结果代码。
message:  错误提示信息。
data:     数据包数据。
