##  文章目的

在成長過程中留下紀錄

## 目錄
1. [這專案在學什麼](https://github.com/miamii11036/Building-a-Boilerplate-by-Bash/blob/main/README.md#%E5%B0%88%E6%A1%88%E4%BB%8B%E7%B4%B9)
2. [在這個專案中學到的指令整理](https://github.com/miamii11036/Building-a-Boilerplate-by-Bash/blob/main/README.md#%E6%8C%87%E4%BB%A4%E7%B5%B1%E6%95%B4)
3. [一些執行過程中遇到的困難與解決方式](https://github.com/miamii11036/Building-a-Boilerplate-by-Bash/blob/main/README.md#%E9%81%87%E5%88%B0%E7%9A%84%E5%9B%B0%E5%A2%83%E8%88%87%E8%A7%A3%E6%B1%BA%E8%BE%A6%E6%B3%95)
4. 學到的教訓
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
