# mono_code
# Wedding Scheduler

## 设置

1. 创建虚拟环境并激活它：
    ```bash
    python -m venv venv
    source venv/bin/activate  # 在Windows上使用 `venv\Scripts\activate`
    ```

2. 安装依赖：
    ```bash
    pip install sqlite3
    ```

3. 将CSV数据加载到数据库：
    ```bash
    python load_csv.py
    ```

## 使用

运行脚本生成婚礼列表：
```bash
python wedding_scheduler.py
