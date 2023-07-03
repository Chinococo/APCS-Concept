tags: ``APCS檢定營隊``
                      

上課重點筆記DAY1
================

Python 使用IDLE
---------------

使用教學
~~~~~~~~

步驟1:開啟Window 下Python IDLE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

|image1| ### 步驟2:開啟新檔案 |image2| ### 步驟3:先保存建立檔案 |image3|
### 步驟4:編寫完成是碼後，開啟執行程式 |image4| ### 步驟5:結果展現
|image5|

Python Basic
------------

特性
~~~~

1. 容易學習(語法簡單)
2. 功能強大(功能已經獏組化)
3. 跨平台(有外部擴充庫可以實作不同軟體)

   -  API : Flask
   -  爬蟲 : selenium
   -  APP : kivy
   -  Form: tkinter ### 功能

4. 資料分析
5. 科學計算
6. 機器學習
7. 網頁設計 ### 基本語法
8. 分號:大部分程式語言使用分號做為結束符號，就如同我們中文中的句號，能讓你知道哪裡要停頓
9. 控制指令:for While if elif
   else這種有可能會需要跳躍行數的程式碼，你要清楚跟他講，如果此條件程式成立，他要做甚麼哪段程式，其他語言是使用大括號
   ex: 如果我考試考得好，父親給我買平板
   如果我考得不好，媽媽給我禁止我玩電腦 if 如果我考試考得好 =>
   父親給我買平板 if 如果我考不好 => 媽媽給我禁止我玩電腦 寫成code

.. code:: python=

   if 如果我考試考得好 :
       父親給我買平板
   if  如果我考不好:
       媽媽給我禁止我玩電腦

Input/output/variable basic
---------------------------

印出資料
~~~~~~~~

Print 裡面放入你想印的數字或文字，就可以印出文字

.. code:: python=

   print(1)
   print(1.2)
   print("123456")

印出多筆資料
~~~~~~~~~~~~

Print
裡面不只可以放一個資料，可以放很多資料，只要用逗點分隔，就能夠在同一行列印出

.. code:: python=

   print(1)
   print(1.2)
   print("123456")

輸入資料
~~~~~~~~

裡面可以放參數，在使用者輸入前先印出文字已提醒使用者該輸入的資料
**重點:回傳必為文字**

.. code:: python=

   print(input())#列印出輸入
   print(type(input()))#理論上會跑出 <class :str>

轉型
~~~~

4大基礎型態
^^^^^^^^^^^

1. integer整數(int)
2. float福點數(float)
3. string文字(str)
4. Boolean布林(bool) 我要她從轉成特定型態: 就用你要的 **型態名稱(資料)**
   ex str(123) => 123這個數字轉成文字 ### 字串操作 ### 字串選告方式

.. code:: python=

   a = '123'
   b = "123"
   c = """123"""
   d = '''123'''#這是錯誤用法

錯誤宣告
~~~~~~~~

**兩兩相對，不可忘記**

.. code:: python=

   a = '123"
   b = '123"
   c = """123'''

取長度 len()
~~~~~~~~~~~~

除了 int float bool不能被取長度，其餘資料型態都有這個方法可以使用

.. code:: python=

   a = 'Hello '
   print(len(a))

使用索引拿取資料
~~~~~~~~~~~~~~~~

|image6| 1.

.. code:: python=

   a = 'Hello artice'
   print(a[1])#[val]=拿第幾個val索引的字元
   print(a[1:2])#[val1,val2]=拿第幾個val1索引的字元到第幾個val2索引以前的全部自元
   print(a[1:2:1])#[val1,val2,val3]=拿第幾個val1索引的字元到第幾個val2索引以前的全部自元，美取完一個數字就像前跳val3步

字串方法
~~~~~~~~

**重點:所有字串方法都不會改到自己本身** |image7| #### capitalize()
正規化文字:把亂七八糟的英文變成，開頭大小，其餘小寫的標準格式 ####
lower() 全部變小寫 #### upper() 全部變大寫 #### islower() 是否全部都小寫
#### upper() 是否全部都大寫 ### count(val) val在這個字串出現過的次數 ###
find(val) val在這個字串出現過的開頭 無找到回傳-1 ### index(val)
val在這個字串出現過的開頭 無找到回傳-1 ### isdigit() 是否是個數字 ##
運算浮 |image8| |image9| |image10| ## 格式化輸出 ### 打法1

.. code:: python=

   a = 'Hello {}'.format("Chino")#若沒寫會自動從做至右分配
   print(a)

打法2
~~~~~

.. code:: python=

   a = 'Hello {0} {0}'.format("Chino","Good")
   print(a)

打法3
~~~~~

.. code:: python=

   b = "Chino"
   a = f'Hello {b}'
   print(a)

If
--

判斷邏輯以控制程式邏輯
**重點:逗號+TAB表示這是這個情況成立才會執行的東西** if 條件: code1 elif
條件2: code2 else: code3 若條件式1 True，執行code1 反之條件式2
True，執行code2 若兩個皆不成立，執行code3
你要告訴她是他要執行的code要在前面加上一個Tab if 一定要最早出現 else if
可以有無限個 else 一定要最晚出現

.. |image1| image:: https://i.imgur.com/uQOrd7q.png
.. |image2| image:: https://i.imgur.com/qdJ22ZI.png
.. |image3| image:: https://i.imgur.com/EMnZaHk.png
.. |image4| image:: https://i.imgur.com/N9Zz3yl.png
.. |image5| image:: https://i.imgur.com/wUu0HbW.png
.. |image6| image:: https://i.imgur.com/Qw3IU0u.png
.. |image7| image:: https://i.imgur.com/ypIPbzE.png
.. |image8| image:: https://i.imgur.com/pqnllrI.png
.. |image9| image:: https://i.imgur.com/J64xpdz.png
.. |image10| image:: https://i.imgur.com/PooPaur.png
