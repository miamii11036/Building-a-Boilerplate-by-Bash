##  文章目的

在成長過程中留下紀錄

## 目錄
1. 這專案在學什麼
2. 在這個專案中學到的指令整理
3. 一些執行過程中遇到的困難與解決方式
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


### 創建類指令 - mkdir,touch
+ ```mkdir <new_folder_name>```：在目前資料夾中，創建名為<new_folder_name>的資料夾。
  + 【變化】
    + ```mkdir <folder_path>/<new_folder_name>```：在目前資料夾中，創建名為<new_folder_name>的資料夾且該資料夾位於<folder_path>裡，不是目前資料夾中。
+ ```touch <new_file_name>```：在目前資料夾中，創建名為<new_file_name>的檔案。
  + 【變化】
    + ```touch <folder_path>/<new_file_name>```：在目前資料夾中，創建名為<new_file_name>的檔案且該檔案位於<folder_path>裡，不是目前資料夾中。
### 移動類指令 - cd
+ ```cd <folder_name>```：將目前狀態移至<folder_name>的資料夾。
  + 【變化】
    + ```cd ..```：將狀態退回前一個資料夾。
    + ```cd ../..```：將狀態退回 前前一個資料夾。

ls -l  -a
echo

rm 
rmdir -r


