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

3. 创建数据库：
    ```bash
    conn = sqlite3.connect('weddings.db')
    cursor = conn.cursor()
    ```

5. 将csv文件导入数据库并创建表：
    ```bash
    cursor.execute('''CREATE TABLE''')
    ```
   
   
## 使用
1. 定义查询函数：
    ```bash
    def get_function():
        cursor.execute('''
        SELECT ***
        ''')
        results = cursor.fetchall()
        return [row[0] for row in results]
    ```



3. 保存查询结果到文件：
    ```bash
    def save_to_file(file_name, data):
        with open(file_name, 'w', encoding='utf-8') as file:
            for item in data:
                file.write(f"{item}\n")
        print(f"Saved data to {file_name}: {data}")
    ```



