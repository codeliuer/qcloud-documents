1) 登录腾讯云控制台，选择无服务器云函数。

2) 在`广州`地域下点击【创建函数】按钮，进入新建函数页面。

3) 填写函数名称`hello-world`，其他配置项保持默认选项即可。

4) 点击【下一步】按钮，进入函数代码编辑页，默认选择【在线编辑】，并在【模版】中选择 `Hello World` 模版。此时，执行方法和代码将填入模版的默认值：

 - 执行方法显示`index.main_handler`。表示无服务器云函数控制台会将此段代码自动保存为`index.py`文件，并压缩该文件上传至 SCF 平台以创建云函数。
 - 函数代码显示以下代码片段：

```
print('Start Hello World function')
def main_handler(event, context):
    print("value1 = " + event['key1'])
    print("value2 = " + event['key2'])
    return event['key1']  #return the value of key "key1"
```
该示例代码将从`event`参数中获取类似以下形式的数据：
```
{
  "key1": "test value 1",
  "key2": "test value 2"
}
```

5) 点击【下一步】，进入触发方式页面。对于此示例代码来说，不需要配置任何触发器，直接点击【完成】按钮。

6) 此时控制台会自动生成代码程序包并上传至 SCF 平台以创建云函数。您可以点击云函数列表页中刚刚创建的`hello-world`函数进入云函数详情页。

