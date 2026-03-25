# Chat Prompt 歷程

1. 我想將這個 workspace 放上我的 github repo 上，請手把手教我。
我的 github 是 https://github.com/sheng-luen-chung

2. 你看得出來，這裏是的 JDK 設定的版本是？

3. 那你解釋一下，這邊為什麼會有 JDK 27 與 JDK 17是怎麼回事？

4. 那我可以設定為 JDK1.8嗎？

5. 你幫我找 jdk 1.8

6. 好，就用這個，你幫我改。
順便也把之前用 JDK 25 編譯的執行檔都刪掉。還有 JDK17應該是沒用的，也刪了

7. 等一下，因為之後這個 repot 在其他的電腦上，我也會希望是在 jdk1.8 上編跡與執行；還有其他的電腦的專案路徑也許不是 C 碟，請也幫我在 settings.json 一併修改

8. 好

9. 但 libaries 也請你不要寫死：

"java.project.referencedLibraries": [
        "c:\\Users\\sheng\\FCPS_eUnits_vscode\\SetupFiles\\karel2_c.jar",
        "c:\\Users\\sheng\\FCPS_eUnits_vscode\\SetupFiles\\xercesImpl.jar"
    ],

10. 那我可以至少在這台電腦上先試過一次，看有沒有問題？
要怎麼試，我要先退出 vs code, 然後？

11. 出了什麼錯？

PS C:\Users\sheng\FCPS_eUnits_vscode>  & 'C:\Program Files\Java\jdk1.8.0_202\bin\java.exe' '-cp' 'C:\Users\sheng\AppData\Local\Temp\cp_281r1ucmtfm0vs617d03pb2yt.jar' 'Lab00'
Exception in thread "main" java.lang.UnsupportedClassVersionError: edu/fcps/karel2/Display has been compiled by a 
more recent version of the Java Runtime (class file version 67.0), this version of the Java Runtime only recognizes class file versions up to 52.0
        at java.lang.ClassLoader.defineClass1(Native Method)
        at java.lang.ClassLoader.defineClass(ClassLoader.java:763)
        at java.security.SecureClassLoader.defineClass(SecureClassLoader.java:142)
        at java.net.URLClassLoader.defineClass(URLClassLoader.java:468)
        at java.net.URLClassLoader.access$100(URLClassLoader.java:74)
        at java.net.URLClassLoader$1.run(URLClassLoader.java:369)
        at java.net.URLClassLoader$1.run(URLClassLoader.java:363)
        at java.security.AccessController.doPrivileged(Native Method)
        at java.net.URLClassLoader.findClass(URLClassLoader.java:362)
        at java.lang.ClassLoader.loadClass(ClassLoader.java:424)
        at sun.misc.Launcher$AppClassLoader.loadClass(Launcher.java:349)
        at java.lang.ClassLoader.loadClass(ClassLoader.java:357)
        at Lab00.main(Lab00.java:13)
PS C:\Users\sheng\FCPS_eUnits_vscode> 

12. 我覺得 Setup files 滿錄中的 karel2_c.jar 誕該是 Java SE 7 寫的

13. 請將我這個 chat 的所有的 prompt 列出在一個 md 檔
