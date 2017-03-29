
## 引入stream处理post和put请求 + 采用Promise构建流式中间件

## 第三课作业小结

> 提交网址 http://jscode.me/t/json-promise-api-server-static-server/982

> 任务11班-陆宇箫
> 柯良勇-已毕业
> 任务3班-陈捷
> 老师-凯敏
> node+vue项目班-杨泽 ==> 笔记较好
> 子威node
> 任务3班-曾萍
> 任务7班-林哲铭
> 任务8班-叶富城
> 任务6班-郭琪琛 Promise实现度较高
> 任务5班-杨承润
> task10-张睿
> 直播10班-彭耀康
> 张磊磊
> 黄锦文
> 费晗
> 任务10班-李杨
> 任务5班-姜杭轩
> 任务7班-周学振
> 任务8班-林伟琨 逻辑清晰+ 笔记记录
> 文韬


------------------------------------------------------

第四节课上课流程安排：

1、第三课Promise回顾【答疑】
2、stream知识 => 处理post请求
3、抽象url-parser
4、Promise抽象中间件模型
5、链式处理static-server、api-server、url-parser中间件。
6、技术答疑



 -------------------------- 课前预习资料-----------------------


- [Promise复习](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise)

- [request对象](https://github.com/nodejs/node/blob/master/doc/api/http.md)

- [stream基本知识](https://github.com/nodejs/node/blob/master/doc/api/stream.md)



-----------------------node的url/querystring模块---------------

> 处理客户端url

[url模块](https://github.com/nodejs/node/blob/master/doc/api/url.md)

- [url模块图解](./3rd-assets/url.png)


> 处理客户端query参数

[querystring模块](https://github.com/nodejs/node/blob/master/doc/api/querystring.md)

```javascript
	querystring.stringify({ foo: 'bar', baz: ['qux', 'quux'], corge: '' })
	// returns 'foo=bar&baz=qux&baz=quux&corge='

	querystring.parse('foo=bar&abc=xyz&abc=123')
	// returns {
	  foo: 'bar',
	  abc: ['xyz', '123']
	}
```