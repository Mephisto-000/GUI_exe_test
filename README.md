# GUI  與 .exe 檔打包測試

- ## GUI 程式碼如下 :

```py
import os
import tkinter as tk

root = tk.Tk() # 建立視窗
root.title("Test") # 建立視窗名
root.geometry("500x700") # 設定視窗大小
root.configure(bg='skyblue') # 設定視窗內顏色
root.mainloop() # 結束視窗
```

- ## 打包成 .exe 檔測試 : 

  - 在 Terminal 中輸入 `pyinstaller -F 檔名.py` : 

    表示生成單個可執行文件

     (Creat a one-folder bundled executable. )

  - 在 Terminal 中輸入 `pyinstaller -F -w 檔名.py` : 

    表示生成單一可執行文件外，並去掉控制台窗

    (Windows and Mac OS X: do not provide a console window for standard i/o. On Mac OS X this also triggers building an OS X .app bundle. On Windows this option will be set if the first script is a ‘.pyw’ file. This option is ignored in *NIX systems.)

- ## 參考網站 : 

  https://pyinstaller.readthedocs.io/en/stable/usage.html

