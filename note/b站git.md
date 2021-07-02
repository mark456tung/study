# CH1
## 版本控制分為分布式和集中式版本控制
* 集中式
   * 所有人都連到一台主機共同開發
   * 如果中央server故障，所有人都不能開發
* 分布式
   * 每個人都在local做版本控制(每個人都有完整的project資料，包括修改紀錄)
   * 遠程庫可以大家共同使用

* 提交到本地庫後才會有紀錄
# CH2
![git](image\git1.png)

git安裝好要先 
>$git config --global user.name \<name>

>$git config --global user.email \<mail>

要讓git管理目錄要先
>cd到要管理目錄

>$git init
# CH3
看狀態
>$git status

存到暫存區
>$git add \<file>

從暫存區刪除
>$ git rm \<file>

提交到本地庫
>$git commit -m "commit" \<file>

簡易版本訊息
>$git reflog

詳細版本訊息
>$git log

版本穿梭
>git reset --hard <版本號>

# CH4 branch

查看分支
>$git branch -v

創建分支
>$git branch \<branch name>

切換分支
>$git checkout \<branch name>

合併分支
>先切換主分支

>$git merge \<要合併的分支>

合併衝突
* 有兩個分支對同一個文件修改
>$git merge <要合併的branc h>

terminal 報錯

開啟那個檔案 然後就會有衝突的部分
 <<<HEAD 當前分支

 當前分支代碼

===

要合併的代碼

 \>>>要合併的分支
 手動修改 

 然後

 >$git add \<file>

 >$git commit "commit" (注意!這裡後面不能有文件名)

 # ch5 git協作

 * 團隊內協作(直接在g)
 push

 clen

 pull

 * 跨團隊協作
 fork

 push到自己的遠程庫

 向原本的申請pull request

 # ch6 github
 git remote -v 看別名

 git remote add \<name>創建別名

 git push/pull  別名 分支

 要邀請別人

 先到git repository 然後Setting -> Manage access -> 
 
 invite a collaborator -> 輸入要邀的人的帳號 -> 旁邊有個
 
 邀請函 複製下來-> 傳給要邀請的人 -> 被邀請的人點進去同意

 * 跨團隊協作

 先fork

生成ssh

# ch7.8 idea 跳過
# ch9 gitee
# gitlab

> ssh-keygen -t rsa -C 


---


LF CRLF 