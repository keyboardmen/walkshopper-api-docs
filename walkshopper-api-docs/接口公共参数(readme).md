#API公共参数文档
该文档描述了客户端访问每个接口都会携带的公共参数以及服务器返回response的基本参数和格式。

##公共请求参数
每个接口都会携带的公共参数。

参数名  | 参数类型  | 是否必填  | 参数说明
:------------- | :------------- | :------------- | :-------------
uniqueId  | string  | Yes  | 标识设备的唯一识别串号
systemName  | string  | Yes  | 设备系统名称
systemVersion  | string  | Yes  | 设备系统版本
deviceType  | string  | Yes  | 设备类型
apiLevel  | string  | Yes  | 接口版本号

##公共返回参数
服务器返回response的基本参数。

参数名  | 参数类型  | 参数说明
:------------- | :------------- | :-------------
retCode  | int  | 200表示成功，其他表示失败
retDesc  | string  | 成功或失败的描述
ret  | object  | 返回内容，服务器的返回内容都会放在ret对应的值中

##公共返回结果示例
~~~
{
	"retCode":200,
	"retDesc":"返回成功"
	"ret":{
		"username":"张三",
		"gender":"m",
		"screenName":"张大胖"
	}
}
~~~