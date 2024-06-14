# prettyPrintJson-Quickstart
```
import json

def pretty_print_json(json_string):
    try:
        # 将字符串解析为JSON对象
        json_object = json.loads(json_string)
        # 使用json.dumps进行格式化输出，设置缩进为4个空格
        formatted_json = json.dumps(json_object, indent=4)
        return formatted_json
    except json.JSONDecodeError as e:
        return f"Invalid JSON string: {e}"

# 示例使用
json_string = '{"name": "John", "age": 30, "city": "New York"}'
formatted_json = pretty_print_json(json_string)
print(formatted_json)
```
