# 青龙面板SDK
开发时间仓促, 海涵
## 使用方法
### 安装
```bash
pip install qinglong-app-sdk
```
### 建立.env文件
```bash
# .env
QL_CLIENT_ID="9DyKR8Aqoa_j12"
QL_CLIENT_SECRET="cXNV4JFNpaTXlgqTdA-sQ8U92323"
```
### 调用
```python
import os
from qinglong_sdk.ql_sdk import QL
from dotenv import load_dotenv
load_dotenv()
url = "http://127.0.0.1:5700"
client_id = os.getenv("QL_CLIENT_ID")
client_secret = os.getenv("QL_CLIENT_SECRET")
ql = QL(url, client_id, client_secret)
ql.test()
```