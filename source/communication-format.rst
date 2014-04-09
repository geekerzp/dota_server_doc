通信格式
========

请求分类
--------
通信分为 **同步请求** 和 **异步请求** :

*同步请求*
  客户端向服务器提交请求，服务器立即进行响应。

*异步请求*
  客户端向服务器提交请求，服务器会将请求进行队列，过段时间进行响应。
  使用异步请求时，服务器必须开启事件处理器。

请求格式
--------
客户端发送请求和服务器响应采用json格式。

请求示例格式如下：

.. code-block:: json
   :linenos:

   {
      'characterId': xxx,
      'roomId': xxx,
      'data': {
        'timestamp': xxx,
        'actorId': xxx,
        'destinaiton': {
          'x1': xxx,
          'y1': xxx,
          'x2': xxx,
          'y2': xxx
        }
      }
   }

不同的请求数据格式有所不同。

响应格式如下：

.. code-block:: json
   :linenos:

   {
      'result': True/False,
      'code': xxx,
      'message': xxx,
      'data': {
        xxx: xxx,
        ...
      }
   }

所有的响应格式相同，其中：

*result*
  请求执行成功或数据正确。

*code*
  结果代码。

*message*
  错误提示信息。

*data*
  数据包数据。



