# mono_code
# Wedding inquiry

## 设置

1. 创建虚拟环境并激活它：
    ```bash
    python -m venv wedding
    source wedding/bin/activate  # 在Windows上使用 `venv\Scripts\activate`
    ```

2. 安装依赖：
    ```bash
    pip install sqlite3（mac内置）
    sqlite3_version: 3.40.1
    ```

3. 将CSV数据添加到新建的数据库：
    ```bash
    python load_csv.py
    ```

## 使用

运行脚本生成婚礼列表：
```bash

