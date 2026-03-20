# jGRASP Setup Instructions

jGRASP, **G**raphical **R**epresentations of **A**lgorithms, **S**tructures, and **P**rocesses for Java, is a lightweight integrated development environment (IDE), created specifically to provide visualizations for improving the comprehensibility of software. See more at [jgrasp.org](https://www.jgrasp.org/index.html).

## Setup

### Java 開發環境需求（VS Code 用戶必讀）

本專案必須使用 **JDK 23 以上（建議 JDK 25）** 進行編譯與執行，因為部分函式庫（如 karel2_c.jar）是以新版 Java 編譯。

請確保：
- 你的電腦已安裝 JDK 23、24 或 25（可至 [Oracle](https://www.oracle.com/java/technologies/downloads/) 或 [Adoptium](https://adoptium.net/temurin/releases/) 下載）。
- 在 VS Code 中，請於「Java: Configure Java Runtime」選擇 JDK 25（或 23 以上）作為專案 JDK。
- 本 repo 的 .vscode/settings.json 已設定 JavaSE-25 為預設，VS Code 會自動偵測本機 JDK 25 路徑。

> 若你在不同電腦或不同磁碟機（如 D:、E:）使用本 repo，只要有安裝 JDK 23 以上並於 VS Code 選擇即可，無需修改任何路徑設定。

#### JRE 說明
JDK 內已包含 JRE，無需額外安裝。VS Code 會自動使用 JDK 內建的 JRE。
如需手動指定 JRE/JDK，請設定系統環境變數 JAVA_HOME 並將 %JAVA_HOME%\bin 加入 PATH。
1. Download the self-extracting installer from the [direct link](https://www.jgrasp.org/dl4g/jgrasp/jgrasp_bdl206_17.exe) (recommended), or from the official download page ([link](https://spider.eng.auburn.edu/user-cgi/grasp/grasp.pl?;dl=download_jgrasp.html)). The installer from the provided direct link was for **Windows** with **Java bundled**.
2. In jGRASP, under the menu *Settings* > *Path-Classpath* > *Workspace*, click on the "*Classpath*" tab. 
    1. Click on "*New*" and browse to the `./Setup Files` folder in this repository. Click on `karel2_c.jar`. Click on "*OK*". 
    2. Click on "*New*" and browse to your `./Setup Files` folder. Click on `xercesImpl.jar`. Click on "*OK*", 
    3. Click on "*Apply*" and then "*OK*".
    
    These steps are **necessary** to run the Karel the Robot exercises and to avoid the error.
3. Enjoy the course!

## Notes
- These materials are mostly credits to **F**airfax **C**ounty **P**ublic **S**chools (FCPS) and **T**homas **J**efferson High School for Science and Technology (TJHSST).
- Visit TJHSST site for more information: [link](https://compsci.sites.tjhsst.edu/CSweb/index.html).
- Visit the official jGRASP site for more information: [link](https://www.jgrasp.org/index.html).