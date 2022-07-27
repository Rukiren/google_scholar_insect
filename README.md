# google scholar Ruki寫的可愛爬蟲使用手冊

**由於 google 不喜歡 Ruki，一直認為我是機器人，所以以下教學都以半自動為主，全自動爬蟲功能還未完善**

## 安裝軟體
1. 點擊打開 "環境安裝.bat" 讓它完整執行
    >![](https://i.imgur.com/vYWzS0N.png)
    > ### 若出現下方附圖情形，表示 python 環境變數未設定，請參考[此連結](https://ithelp.ithome.com.tw/articles/10257693)修正
    > ![](https://i.imgur.com/R2ZxBNQ.png)

## 軟體基礎設定
1. 打開 Visual Studio Code
    > 1. 使用右下角搜尋尋找 Visual Studio Code
    > ![](https://i.imgur.com/qUq0seq.png)
    > ![](https://i.imgur.com/4wgeQhq.png)
    > 
2. 打開檔案
     > 左上角 "檔案" -> "開啟資料夾"
     > 快捷鍵:Ctrl+k,Ctrl+O(按完K再按O)
3. 找到資料夾位置
4. 點擊選擇資料夾 
    > ![](https://i.imgur.com/xJ4nrJ2.png)
5. 點開 no_google.main,py
    > ![](https://i.imgur.com/7uTeZXJ.png)
    
6. 修改各項資料儲藏位置
    > 第 19 行為 excel 的名稱，請將 new.xlsx 替換成您的 excel 名稱
    > 第 20 行為 excel 中表單的名稱，請記得替換成您的表單名稱
    > 第 21 到 25 行中數字代表要將資料存在 excel 中第幾行
    > 假設 excel 的 A 要存標題，就將標題的 3 改成 1
    > 假設 excel 的 B 要存標題，就將標題的 3 改成 2
    > 以此類推修改
    > 
    > ![](https://i.imgur.com/sgyP8M9.png)

7. 修改開始列數
    > 點開 time.txt
    > 將裡面數字修改為您要開始儲存的列數
    > 若從第 6 行開始就打 6 並存檔(Ctrl+S)
    > ![](https://i.imgur.com/ogbbGsH.png)

## 實際使用
- 點擊右上角播放鍵運行程式
     ![](https://i.imgur.com/DODGWua.png)
- 確定出現圖片中框起部分
     ![](https://i.imgur.com/KnN2A4c.png)
- 在 Visual Studio Code 中打開 html.txt
    ![](https://i.imgur.com/OFlcIQM.png) 
- 打開 google scholar 搜尋指定關鍵字、年份等
    ![](https://i.imgur.com/ZxFSiXG.png)
- 打開檢查
    - 空白處右鍵，最下方有個檢查點下去
    - 快捷鍵: F12
    - 會看到右邊這個酷東西
     ![](https://i.imgur.com/m4jUGx2.png)
- 點圖片中圈起來的箭頭
 ![](https://i.imgur.com/hruZ62g.png)
 ![](https://i.imgur.com/AuNROlo.png)
- 然後移動到左邊的搜尋畫面中，直到出現如圖片的畫面
 ![](https://i.imgur.com/yqzpIBZ.png)
 
- 滑鼠左鍵按一下

- 會在左方自動幫你找到我們需要複製的 html
 ![](https://i.imgur.com/c95m7EU.png)

- 對這行右鍵，然後選擇 Copy -> Copy outerHTML
- 回到 Visual Studio Code 中的 html.txt
- 貼上並存檔
 ![](https://i.imgur.com/MKKQvSu.png)

- 鼠標移動到下方終端機視窗中，左鍵按一下，按一下 Enter
 ![](https://i.imgur.com/bI0zdym.png)

> 若須繼續加上下一頁的資料請重複"複製 Html -> 貼上到 html.txt -> 按 Enter"
> 若需結束請輸入 END 後按 Enter
> **不要直接關檔案或者強制結束**

- 可以打開 Excel 看一下資料儲存的狀況
 ![](https://i.imgur.com/7ROm9QO.png)
    > 若無抓取到作者資料會整行標記橘色
    > 若無抓取到年分會自動標記 None 並填入黃色
    > 若抓取到的期刊名稱不完整，會標記黃色
    
## 錯誤排除
1. 程式執行時沒有關閉 Excel
![](https://i.imgur.com/6qt6TaT.png)
    - 解決辦法:關掉 Excel
    
2. time.txt(開始列數)無資料
![](https://i.imgur.com/9kGEVlB.png)
    - 若程式不正常關閉會導致當前列數沒有儲存到 time.txt
    - 解決辦法:確定當前 excel 的列數，手動輸入 time.txt 並存檔

3. 其他未知問題
    - 解決辦法: 截圖錯誤訊息，並打包所有檔案 mail 給 Ruki
    - Mail: houpig1@gmail.com
