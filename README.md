# UNIX_HW1_C-Steve:透過寫一個text adventure game來學習UNIX's directory structure

### 文本冒險遊戲(text adventure game) & UNIX目錄結構(UNIX's directory structure)的相似性:
+ **文本冒險遊戲 :**
    + 在各個房間內移動，你可以查看跟移動物品。
    + 有著上鎖的門，如果沒有鑰匙或道具就無法進入。
    + 有隱藏道具。
+ **UNIX目錄結構 :**
    + 在目錄間，你可以查看跟移動物品檔案。
    + 可以有特殊限制，拒絕你的存取。
    + 有隱藏文件。
## 前言 :
要重寫一個叫Dunnet的遊戲，因為Dunnet這個遊戲是從Emac的文字編輯器生出來的，<br /> 
裡面很多Key Code 也適用於UNIX基本命令，C+覺得這樣學UNIX很棒棒。
### Dunnet
+ **Dunnet**是一個文字冒險遊戲，在一開始，你站在泥濘的道路的盡頭，這和普通的冒險遊戲差不多，<br /> 但是，接下來，這個遊戲就會暴露出它奇怪 ~鬼畜~ 的本質。(有興趣請自行查詢)
    + 這個遊戲存在於emac中，所以如果想要玩可以照下面的指令下載emac。
    + 要玩這個遊戲可以打`emacs -batch -l dunnet`(下載完emac後)
    + the dunnet game is going to be run from the UNIX command prompt, not from within the emacs screen.   
### 下載 emac 文字編輯器
+ 指令:`sudo apt-get install emacs`
    + To verify that you have emacs, type `emacs` .If it doesn't run, then install it. <br /> Once emacs is running, close it by typing Ctrl-x, Ctrl-c. <br /> I only had you open it to test if it was installed.
      
## 具體方向 :
第一次作業，我們要**建一些目錄與檔案**，對應Dunnet遊戲的一部分。<br /> 
(下一次我們會用**aliases(指令別名)** 來做遊戲指令) <br />
一旦完成創建，你就可以建壓縮檔並繳交。

## Let's Start!!!!!!
如果你已經看過C+傳的README的話，你一定已經解壓縮完而且有個資料夾叫**PA1**，讓我們來看一下裡面的東西 : <br />
### explanatoryWalkthrough.txt
+ 解釋要怎麼玩 Dunnet Game (這部分會是本次作業的重點，但在看之前請先看完**README**)
### savedgame
+ 用來加載我們會用到的部分(在**explanatoryWalkthrough.txt**會說要怎麼用這個檔案)
### PA1assignment.txt 
+ 描述本次作業一的細節部分(請先看完**explanatoryWalkthrough.txt** )
### descriptions.txt and objects.txt
+ 這兩個檔案有你在這次作業裡需要放進不同檔案裡的文字敘述，怎麼做的詳細描述在**PA1assignment.txt**裡
### gradingPolicy.txt
+ 講解評分規則，C+在課堂上講的東東 
+ 裡面還有說作業的最低基本要求，達不到也是0分
### findYourOutput.exe
+ 它可以幫你建一個Output的list，可以跟**expectedOutput**這個檔案比較，以測試出有沒有達到最低基本要求。(要如何測試的方法在**gradingPolicy.txt**裡。)
### expectedOutput
+ 本次作業的標準，在**PA1assignment.txt**裡有解釋要怎麼check你的答案
+ 若你點開此檔，你會看到所有你在這次作業將會建立的檔案跟目錄。
+ 這裡我看不懂也懶得翻了~累累~，放原文:
    + This listing
has a nice feature, that each individual directory appears in one place. What
do I mean? Well consider the receivingRoom, it has an axe and a shovel (among
other things). It also has a door to the east. the find command alphabetizes
these things, so "axe" comes before "e" which comes before "shovel". This is
not the best ordering, because it means the axe and shovel do not appear near
each other when you type: find . -name "*".  But they do appear near each
other in the expectedOutput file. (And in the output of findYourOutput.txt.)

## 結尾
C+給的**README**結束了，再來去讀(2)**explanatoryWalkthrough.txt**吧 :)
然後(3)**PA1assignment.tx**
再(4)**gradingPolicy.txt**
