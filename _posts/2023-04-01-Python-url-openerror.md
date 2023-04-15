---
layout:       post
title:        "Python-URL-OpenError"
author:       "Lianz"
header-style: text
catalog:      true
tags:
    - URL
    - error
    - Python
---

> 关于如何解决以下报错：urllib.error.URLError: <urlopen error [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self signed certificate in certificate chain (_ssl.c:997)>

通过URL链接数据集

```
# Get the IRIS dataset
url = "https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data"
data = pd.read_csv(url, names=['sepal length', 'sepal width', 'petal length', 'petal width', 'target'])
```

但是显示报错

```
urllib.error.URLError: <urlopen error [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self signed certificate in certificate chain (_ssl.c:997)>
```

然后通过以下方式解决，全局取消证书验证

```
import ssl
ssl._create_default_https_context = ssl._create_unverified_context
```



