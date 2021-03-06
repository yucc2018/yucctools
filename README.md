## yucctools

常用的工具分享。可以方便的调用本工具去记录日志等。


### 1. 安装

方法一：直接使用pip安装

```python
pip install yucctools
```

方法二：国内pip有时较慢，可以指定使用清华源安装

```python
pip install yucctools -i https://pypi.tuna.tsinghua.edu.cn/simple
```

### 2. 使用示例

#### 2.1 日志工具

可以方便的去初始化记录日志，并记录日志，样例：

```python
# 导入包
import yucctools as yt

# 初始化logger实例
logger = yt.logger(filepath='test.log')

# 记录信息，只要这么调用就可以使用了
# 记录一条debug级别的日志
logger.info('this is a debug levle log.')
# 记录一条info级别的日志
logger.info('this is a info level log.')
# 记录一条warning级别的日志记录
logger.warning('this is a warning level log.')
# 记录一条error级别的日志记录
logger.error('this is a error level log.')
# 记录一条critical级别的日志记录
logger.critical('this is a critical level log.')
```

#### 2.2 小数格式工具

方便进行小数展示

```python
import yucctools as yt

# 自动保留四位小数，转换成str
num1 = yt.digit_format(2.5623478234)

# 设定保留2位小数，转换成str
num2 = yt.digit_format(3.8234234234, n=2)
```


### 附录

github网页：https://github.com/yucc2018/yucctools

pypi网页：https://pypi.org/project/yucctools/
