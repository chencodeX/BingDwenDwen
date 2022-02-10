# BingDwenDwen
Use python to draw BingDwenDwen and package them into executable files

## Usage

Modify line 717 to change the text you want to customize, if you don't need it, you can comment it

```python
turtle.write("XXX", font=('KaiTi', 16))
```

## package

install pyinstaller package
```sh
python -m pip install -i http://pypi.douban.com/simple --trusted-host pypi.douban.com pyinstaller
```

generate executable
```sh
cd workspace
pyinstaller -F -w -i  ./logo.ico BingDwenDwen.py --noconsole
# logo.ico file is your icon,if not,cancel -i 
```
After the packaging is successful, the executable file exists in the **dist** folder
