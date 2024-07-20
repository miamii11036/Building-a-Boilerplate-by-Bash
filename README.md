##  文章目的

在成長過程中留下紀錄

## 目錄
1. [這專案在學什麼](https://github.com/miamii11036/Building-a-Boilerplate-by-Bash/blob/main/README.md#%E5%B0%88%E6%A1%88%E4%BB%8B%E7%B4%B9)
2. [在這個專案中學到的指令整理](https://github.com/miamii11036/Building-a-Boilerplate-by-Bash/blob/main/README.md#%E6%8C%87%E4%BB%A4%E7%B5%B1%E6%95%B4)
3. [一些執行過程中遇到的困難與解決方式](https://github.com/miamii11036/Building-a-Boilerplate-by-Bash/blob/main/README.md#%E9%81%87%E5%88%B0%E7%9A%84%E5%9B%B0%E5%A2%83%E8%88%87%E8%A7%A3%E6%B1%BA%E8%BE%A6%E6%B3%95)

****
# 專案介紹
在Linux系統中，用Bash shell創建網站模板。以此學習、熟悉Bash的基礎指令，如搜尋類指令、創建類指令、移動類指令、顯示類指令、刪除類指令

# 指令統整
### 搜尋類指令 - find
+ ```find```：以數狀圖的形式顯示目前資料夾中的所有資料。
+ 【標籤】
  + ```find -name <file_name>``` ：在目前資料夾中，顯示與<file_name>相同名稱的檔案，並以數狀圖形式呈現。
+ 【變化】
  + ```find <folder_name>```：以數狀圖的形式顯示<folder_name>資料夾中的所有資料。


### 創建類指令 - mkdir, touch
+ ```mkdir <new_folder_name>```：在目前資料夾中，創建名為<new_folder_name>的資料夾。
  + 【變化】
    + ```mkdir <folder_path>/<new_folder_name>```：在目前資料夾中，創建名為<new_folder_name>的資料夾且該資料夾位於<folder_path>裡，不是目前資料夾中。
+ ```touch <new_file_name>```：在目前資料夾中，創建名為<new_file_name>的檔案。
  + 【變化】
    + ```touch <folder_path>/<new_file_name>```：在目前資料夾中，創建名為<new_file_name>的檔案且該檔案位於<folder_path>裡，不是目前資料夾中。
### 移動類指令 - cd, mv
+ ```cd <folder_name> 或 <file_name>```：將目前狀態移至<folder_name> 或 <file_name> 的資料夾 或 檔案。
  + 【變化】
    + ```cd ..```：將狀態退回前一個資料夾。
    + ```cd ../..```：將狀態退回 前前一個資料夾。
+ ```mv <file_name> <folder_path/folder_name>```將名為<file_name>的檔案，從目前的資料夾中移至 <folder_path/folder_name>的資料夾中。
  
> mv是具有兩種功能的指令，一個是移動檔案位置，另一個是更改檔案名稱
>
> ```mv <file_name> <new_file_name>```：將名為<file_name>的檔案，重新命名成<new_file_name>。


### 顯示類指令 - ls, echo, more
+ ```ls```：列出目前資料夾中，所有沒有被隱藏起來的檔案與資料夾。
  + 【標籤】
     + ```ls -a```：列出目前資料夾中，所有的檔案與資料夾(包含被隱藏的)
     + ```ls -l```：在目前資料夾中，以條列式呈現，所有沒有被隱藏起來的檔案與資料夾，並且會顯示其基本資訊。
+ ```echo <text>```：讓終端顯示出<text>的內容。
  + 【變化】
      + ```echo <text> >> <file_name>```：在名為<file_name>檔案中，輸入<text>的內容。
+ ```more <file_name>```：將<file_name>的檔案資料以一頁一頁的方式顯示在終端，方便閱讀。
### 刪除類指令 - rm, rmdir
+ ```rm <file_name>```：在目前資料夾中，移除名為<file_name>的檔案。
  + 【變化】
    + ```rm <folder_name>/<file_name>```：在目前資料夾中，移除<folder_name>資料夾中的<file_name>檔案
+ ```rmdir <folder_name>```：在目前資料夾中，移除名為<folder_name>的資料夾，且該資料夾不能含有其他檔案。
  + 【標籤】
    + ```rmdir -r <folder_name>```在目前資料夾中，移除名為<folder_name>的資料夾，不論該資料夾有沒有其他檔案。
    
# 遇到的困境與解決辦法
要完成這個專案時遇到滿多問題的，但這些問題並不是發生在專案本身；這專案其實很簡單直白，甚至連其裡頭使用的英文單字也都很簡單，從頭到尾也就一直使用上述列的指令而已。真正難的點是如何開啟這個學習專案。

FreeCodeCamp的relational Database相關專案的建設基礎是建立在Gitpod平台上，藉由Gitpod提供的個人workspace服務來執行並紀錄專案的進度，但Gitpod兩年前突然設立手機驗證系統，為了避免Gitpod的資源被一堆免費帳號過度浪費，但它的手機驗證系統其實滿其奇特的，不是傳簡訊驗證而是打電話，而恰巧我的國家電信業者好像不支援此服務🥲，所以試了很多隻門號都無法通過驗證，所以我就上網查查解決辦法，便發現還有透過在本機來執行專案的方法(ps：此方法不能在freecodecamp帳號上留下紀錄🥲)，也是我認識Linux、Docker的開端。

freecodecamp的relational database的相關實作專案是以Linux作業系統為基礎開發的學習程式軟體，所以要開始學習需先學習如何架設Docker container，需要用的的軟體有 Docker engine、VScode、Git。
+ Docker engine：是一種開源的主機軟體，能支援多種作業系統(如Windows、各種Linux發行版)並在上面架設、執行多個Docker Containers，所以能把Docker engine視為一種管理、執行Docker Containers的平台軟體(但不是直接管理，而是透過Docker Image)。
> Docker Container是一種能夠安全、快速、簡單地執行各種程式的工具，每個container都具有以下特性
> 1. 隔離性：每個container都是獨立互不影響的，並且與主機系統保持一定的"安全距離"(並不能完全避免惡意程式的攻擊，所以還是不要隨意下載未知軟體)。
> 2. 輕量性：container共用主機系統的核心，所以能夠快速啟動並且佔用資源較少。
> 3. 移植性：container包含運行應用程式所需要的所有東西，所以只要環境支援Docker就能執行container所含的應用程式。
> 4. 版本控制：container是架設在Docker Image上，而Image具有 只能被讀取不能被更改、層次結構的版本紀錄，所以藉由選擇Image的版本來回到"上一步"。
+ VScode：是一種開源的程式碼編輯器，能夠跨平臺、安裝各種擴展軟件(如執行此專案會用到的Dev container)、支援Git能直接版本控制、整合式終端能直接用各種程式語言編碼，超好用神器，偉哉！！Microsoft爸爸！
+ Git：是一種開源的分散式版本控制系統，藉由創建儲存庫來紀錄保存文件與其更改歷史，還能建立遠端儲存庫讓多個使用端遠端下載。

### 執行學習專案的方法
1. 開啟Git終端，將freecodecamp的Github學習專案儲存庫複製至本機。(遠端儲存庫連結：https://github.com/freeCodeCamp/rdb-alpha)
2. 開啟本機的終端，將目前路徑導航至剛剛複製的資料夾(rdb-alpha)：輸入 ```cd rdb-alpha```，讓原本的狀態 C:\users 變成C:\users\rdb-alpha) (前提是要將rdb-alpha資料夾儲存在使用者資料夾中，才能成功導航。當然，你也能儲存至別的資料夾並導航過去，反正要讓終端找到這個rdb-alpha資料夾就是了)
3. 輸入 ```code . ```，會自動啟動VSCode
4. 在VSCode中，按下ctrl + shift + P (或直接在上端的搜尋欄點選```show and run commands```)打開命令面板，輸入並執行```Dev Containers: Rebuild and Reopen in Container```，會自動下載並執行Dev Containers (沒有就手動下載並再次輸入命令)，之後系統會自動建立Docker Image，並在container中安裝CodeRoad
5. 在命令面板輸入 ```CodeRoad: start```。VSCode會執行CodeRoad程式
6. 在CodeRoad按下```Start New Tutorial```，點擊URL按鈕，貼上要學習的項目的tutorial.json檔案之URL，就能開始學習了。


