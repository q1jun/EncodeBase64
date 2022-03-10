# base64隐写python脚本

根据base64的填充规则，向填充我给写入或从中读出隐藏信息

## 0x01 使用方法

**写信息**：
```bash
❯ python3 enStego.py source.txt stego.txt 「隐写信息」
```

**读信息**:
```bash
❯ python3 deStego.py stego.txt
```

## 0x02 函数说明

```python
def deStego(stegoFile)
```
从隐写文件stegoFile提取字符串

```python
def enStego(sourceFile, stegoFile, message)
```
根据源文件sourceFile隐写字符串message,base64保存到stegoFile。
