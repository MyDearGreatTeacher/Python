# Python standard library

>* Python有許多內建的函式庫(可以寫成幾本書)
>* 不需安裝即可使用(第三方套件需要安裝==>Tensorflow/PyTorch)
>* 使用時請import載入相關函式庫即可
>* 

# 第三方套件參考書
```
Python 3標準庫 THE PYTHON 3 STANDARD LIBRARY BY EXAMPLE

https://docs.python.org/3/
連上去看看有許多範例 https://pymotw.com/3/
```
```
第1章 文本 1
1.1 string：文本常量和範本 1
1.1.1 函數 1
1.1.2 範本 2
1.1.3 高級範本 3
1.1.4 Formatter 5
1.1.5 常量 5
1.2 textwrap：格式化文字段落 6
1.2.1 示例數據 6
1.2.2 填充段落 7
1.2.3 去除現有的縮進 7
1.2.4 結合dedent和fill 8
1.2.5 縮進塊 8
1.2.6 首行凸排 10
1.2.7 截斷長文本 10
1.3 re：規則運算式 11
1.3.1 查找文本中的模式 11
1.3.2 編譯運算式 12
1.3.3 多重匹配 13
1.3.4 模式語法 14
1.3.5 限制搜索 22
1.3.6 用組解析匹配 24
1.3.7 搜索選項 29
1.3.8 前向或後向 35
1.3.9 自引用運算式 38
1.3.10 用模式修改字串 42
1.3.11 利用模式拆分 44
1.4 difflib：比較序列 46
1.4.1 比較文本體 47
1.4.2 無用資料 49
1.4.3 比較任意類型 50

第2章 資料結構 52
2.1 enum：枚舉類型 53
2.1.1 創建枚舉 53
2.1.2 反覆運算 53
2.1.3 比較Enum 54
2.1.4 唯一枚舉值 55
2.1.5 通過程式設計創建枚舉 56
2.1.6 非整數成員值 58
2.2 collections：容器資料類型 60
2.2.1 ChainMap：搜索多個字典 60
2.2.2 Counter：統計可散列的物件 63
2.2.3 defaultdict：缺少的鍵返回一個預設值 66
2.2.4 deque：雙端佇列 67
2.2.5 namedtuple：帶命名欄位的元組子類 70
2.2.6 OrderedDict：記住向字典中增加鍵的順序 74
2.2.7 collections.abc：容器的抽象基類 76
2.3 陣列：固定類型資料序列 78
2.3.1 初始化 78
2.3.2 處理陣列 79
2.3.3 陣列和檔 79
2.3.4 候選位元組順序 80
2.4 heapq：堆排序演算法 81
2.4.1 示例數據 81
2.4.2 創建堆 82
2.4.3 訪問堆的內容 83
2.4.4 堆的數據極值 85
2.4.5 高效合併有序序列 85
2.5 bisect：維護有序列表 86
2.5.1 有序插入 86
2.5.2 處理重複 87
2.6 queue：執行緒安全的FIFO實現 88
2.6.1 基本FIFO佇列 88
2.6.2 LIFO佇列 89
2.6.3 優先佇列 89
2.6.4 構建一個多執行緒播客客戶程式 90
2.7 struct：二進位資料結構 93
2.7.1 函數與Struct類 93
2.7.2 打包和解包 93
2.7.3 位元組序 94
2.7.4 緩衝區 95
2.8 weakref：對象的非永久引用 96
2.8.1 引用 96
2.8.2 引用回檔 97
2.8.3 最終化物件 98
2.8.4 代理 100
2.8.5 緩存對象 101
2.9 copy：複製對象 103
2.9.1 淺副本 103
2.9.2 深副本 104
2.9.3 定制複製行為 105
2.9.4 深副本中的遞迴 106
2.10 pprint：美觀列印資料結構 107
2.10.1 列印 108
2.10.2 格式化 108
2.10.3 任意類 109
2.10.4 遞迴 110
2.10.5 限制嵌套輸出 110
2.10.6 控制輸出寬度 111

第3章 演算法 113
3.1 functools：管理函數的工具 113
3.1.1 修飾符 113
3.1.2 比較 119
3.1.3 緩存 122
3.1.4 縮減資料集 125
3.1.5 泛型函數 127
3.2 itertools：反覆運算器函數 129
3.2.1 合併和分解反覆運算器 129
3.2.2 轉換輸入 132
3.2.3 生成新值 133
3.2.4 過濾 135
3.2.5 資料分組 138
3.2.6 合併輸入 139
3.3 operator：內置操作符的函數介面 144
3.3.1 邏輯操作 144
3.3.2 比較操作符 145
3.3.3 算術操作符 145
3.3.4 序列操作符 146
3.3.5 原地操作符 148
3.3.6 屬性和元素“獲取方法” 148
3.3.7 結合操作符和定制類 150
3.4 contextlib：上下文管理器工具 151
3.4.1 上下文管理器API 151
3.4.2 上下文管理器作為函數修飾符 153
3.4.3 從生成器到上下文管理器 154
3.4.4 關閉打開的控制碼 156
3.4.5 忽略異常 157
3.4.6 重定向輸出流 158
3.4.7 動態上下文管理器棧 159

第4章 日期和時間 166
4.1 time：時鐘時間 166
4.1.1 比較時鐘 166
4.1.2 牆上時鐘時間 167
4.1.3 單調時鐘 168
4.1.4 處理器時鐘時間 169
4.1.5 效能計數器 170
4.1.6 時間組成 170
4.1.7 處理時區 171
4.1.8 解析和格式化時間 172
4.2 datetime：日期和時間值管理 174
4.2.1 時間 174
4.2.2 日期 175
4.2.3 timedelta 177
4.2.4 日期算數運算 178
4.2.5 比較值 179
4.2.6 結合日期和時間 179
4.2.7 格式化和解析 180
4.2.8 時區 182
4.3 calendar：處理日期 183
4.3.1 格式化示例 183
4.3.2 當地語系化環境 185
4.3.3 計算日期 186

第5章 數學運算 188
5.1 decimal：定點數和浮點數的數學運算 188
5.1.1 Decimal 188
5.1.2 格式化 189
5.1.3 算數運算 190
5.1.4 特殊值 191
5.1.5 上下文 192
5.2 fractions：有理數 196
5.2.1 創建Fraction實例 197
5.2.2 算數運算 198
5.2.3 近似值 199
5.3 random：偽亂數產生器 199
5.3.1 生成亂數 200
5.3.2 指定種子 200
5.3.3 保存狀態 201
5.3.4 隨機整數 202
5.3.5 選擇隨機元素 203
5.3.6 排列 203
5.3.7 採樣 205
5.3.8 多個並發生成器 205
5.3.9 SystemRandom 206
5.3.10 非均勻分佈 207
5.4 math：數學函數 208
5.4.1 特殊常量 208
5.4.2 測試異常值 208
5.4.3 比較 210
5.4.4 將浮點值轉換為整數 212
5.4.5 浮點值的其他表示 213
5.4.6 正號和負號 214
5.4.7 常用計算 215
5.4.8 指數和對數 218
5.4.9 角 222
5.4.10 三角函數 224
5.4.11 雙曲函數 226
5.4.12 特殊函數 227
5.5 statistics：統計計算 228
5.5.1 平均值 228
5.5.2 方差 230

第6章 檔案系統 232
6.1 os.path：平臺獨立的檔案名管理 233
6.1.1 解析路徑 233
6.1.2 建立路徑 236
6.1.3 規範化路徑 237
6.1.4 檔時間 238
6.1.5 測試檔 238
6.2 pathlib：檔案系統路徑作為物件 240
6.2.1 路徑表示 240
6.2.2 建立路徑 240
6.2.3 解析路徑 242
6.2.4 創建具體路徑 243
6.2.5 目錄內容 244
6.2.6 讀寫文件 246
6.2.7 管理目錄和符號連結 246
6.2.8 檔案類型 247
6.2.9 檔案屬性 248
6.2.10 許可權 250
6.2.11 刪除 250
6.3 glob：檔案名模式匹配 252
6.3.1 示例數據 252
6.3.2 萬用字元 252
6.3.3 單字元萬用字元 253
6.3.4 字元區間 253
6.3.5 轉義元字元 254
6.4 fnmatch：UNIX式glob模式匹配 254
6.4.1 簡單匹配 254
6.4.2 過濾 255
6.4.3 轉換模式 256
6.5 linecache：高效讀取文字檔 257
6.5.1 測試資料 257
6.5.2 讀取特定行 257
6.5.3 處理空行 258
6.5.4 錯誤處理 258
6.5.5 讀取Python原始檔案 259
6.6 tempfile：暫存檔案系統物件 260
6.6.1 暫存檔案 260
6.6.2 命名檔 262
6.6.3 周邊同作文件 262
6.6.4 臨時目錄 263
6.6.5 預測名 264
6.6.6 暫存檔案位置 264
6.7 shutil：高層檔操作 265
6.7.1 複製檔 265
6.7.2 複製檔中繼資料 268
6.7.3 處理目錄樹 269
6.7.4 查找文件 271
6.7.5 歸檔 272
6.7.6 檔案系統空間 275
6.8 filecmp：比較文件 276
6.8.1 示例數據 276
6.8.2 比較文件 278
6.8.3 比較目錄 279
6.8.4 在程式中使用差異 280
6.9 mmap：記憶體映射檔 283
6.9.1 讀文件 284
6.9.2 寫文件 285
6.9.3 規則運算式 286
6.10 codecs：字串編碼和解碼 287
6.10.1 Unicode入門 287
6.10.2 處理文件 289
6.10.3 位元組序 291
6.10.4 錯誤處理 293
6.10.5 編碼轉換 295
6.10.6 非Unicode編碼 296
6.10.7 增量編碼 297
6.10.8 Unicode資料和網路通信 299
6.10.9 定義定制編碼 301
6.11 io：文本、十進位和原始流I/O工具 307
6.11.1 記憶體中的流 307
6.11.2 為文本資料包裝位元組流 308

第7章 資料持久存儲與交換 310
7.1 pickle：對象序列化 311
7.1.1 編碼和解碼字串中的資料 311
7.1.2 處理流 312
7.1.3 重構物件的問題 313
7.1.4 不可醃制的物件 314
7.1.5 迴圈引用 316
7.2 shelve：物件的持久存儲 318
7.2.1 創建一個新shelf 318
7.2.2 寫回 319
7.2.3 特定shelf類型 320
7.3 dbm：UNIX鍵-值資料庫 320
7.3.1 資料庫類型 321
7.3.2 創建一個新資料庫 321
7.3.3 打開一個現有資料庫 322
7.3.4 錯誤情況 322
7.4 sqlite3：嵌入式關聯式資料庫 323
7.4.1 創建資料庫 323
7.4.2 獲取資料 326
7.4.3 查詢中繼資料 327
7.4.4 行對象 328
7.4.5 在查詢中使用變數 329
7.4.6 批量載入 331
7.4.7 定義新的列類型 331
7.4.8 確定列類型 334
7.4.9 事務 336
7.4.10 隔離級別 338
7.4.11 記憶體中的資料庫 341
7.4.12 匯出資料庫內容 341
7.4.13 在SQL中使用Python函數 342
7.4.14 帶規則運算式的查詢 344
7.4.15 定制聚集 345
7.4.16 執行緒和連接共用 346
7.4.17 限制對資料的訪問 347
7.5 xml.etree.ElementTree：XML操縱API 349
7.5.1 解析XML文檔 349
7.5.2 遍歷解析樹 350
7.5.3 查找文檔中的節點 351
7.5.4 解析節點屬性 352
7.5.5 解析時監視事件 354
7.5.6 創建一個定制樹構造器 356
7.5.7 解析串 357
7.5.8 用元素節點構造文檔 359
7.5.9 美觀列印XML 359
7.5.10 設置元素屬性 360
7.5.11 由節點列表構造樹 362
7.5.12 將XML序列化至一個流 364
7.6 csv：逗號分隔值文件 366
7.6.1 讀文件 366
7.6.2 寫文件 367
7.6.3 方言 368
7.6.4 使用欄位名 373

第8章 資料壓縮與歸檔 375
8.1 zlib：GNU zlib壓縮 375
8.1.1 處理記憶體中的資料 375
8.1.2 增量壓縮與解壓縮 377
8.1.3 混合內容流 378
8.1.4 校驗和 378
8.1.5 壓縮網路資料 379
8.2 gzip：讀寫GNU zip文件 382
8.2.1 寫壓縮檔 382
8.2.2 讀壓縮資料 384
8.2.3 處理流 385
8.3 bz2：bzip2壓縮 386
8.3.1 記憶體中的一次性操作 386
8.3.2 增量壓縮和解壓縮 388
8.3.3 混合內容流 388
8.3.4 寫壓縮檔 389
8.3.5 讀壓縮檔 390
8.3.6 讀寫Unicode數據 391
8.3.7 壓縮網路資料 392
8.4 tarfile：tar歸檔訪問 395
8.4.1 測試tar檔 396
8.4.2 從歸檔讀取中繼資料 396
8.4.3 從歸檔抽取檔 397
8.4.4 創建新歸檔 399
8.4.5 使用候選歸檔成員名 399
8.4.6 從非檔源寫資料 400
8.4.7 追加到歸檔 400
8.4.8 處理壓縮歸檔 401
8.5 zipfile：ZIP歸檔訪問 402
8.5.1 測試ZIP檔 402
8.5.2 從歸檔讀取中繼資料 402
8.5.3 從歸檔抽取歸檔檔 404
8.5.4 創建新歸檔 404
8.5.5 使用候選歸檔成員名 406
8.5.6 從非檔源寫資料 406
8.5.7 利用ZipInfo實例寫資料 407
8.5.8 追加到文件 407
8.5.9 Python ZIP歸檔 408
8.5.10 限制 410

第9章 加密 411
9.1 hashlib：密碼散列 411
9.1.1 散列演算法 411
9.1.2 示例數據 412
9.1.3 MD5示例 412
9.1.4 SHA1示例 412
9.1.5 按名創建散列 413
9.1.6 增量更新 413
9.2 hmac：密碼消息簽名與驗證 414
9.2.1 消息簽名 415
9.2.2 候選摘要類型 415
9.2.3 二進位摘要 416
9.2.4 消息簽名的應用 416

第 10 章 使用進程、執行緒和協程提供併發性 420
10.1 subprocess：創建附加進程 420
10.1.1 運行外部命令 421
10.1.2 直接處理管道 425
10.1.3 連接管道段 427
10.1.4 與其他命令交互 428
10.1.5 進程間傳遞信號 430
10.2 signal：非同步系統事件 434
10.2.1 接收信號 434
10.2.2 獲取已註冊的處理器 435
10.2.3 發送信號 436
10.2.4 鬧鈴 436
10.2.5 忽略信號 437
10.2.6 信號和執行緒 438
10.3 threading：進程中管理併發操作 440
10.3.1 Thread對象 440
10.3.2 確定當前執行緒 441
10.3.3 守護與非守護執行緒 442
10.3.4 枚舉所有執行緒 444
10.3.5 派生執行緒 445
10.3.6 計時器執行緒 447
10.3.7 執行緒間傳送信號 447
10.3.8 控制資源訪問 449
10.3.9 同步執行緒 453
10.3.10 限制資源的併發訪問 456
10.3.11 執行緒特定的資料 457
10.4 multiprocessing：像執行緒一樣管理進程 459
10.4.1 multiprocessing基礎 460
10.4.2 可導入的目標函數 461
10.4.3 確定當前進程 461
10.4.4 守護進程 462
10.4.5 等待進程 463
10.4.6 終止進程 465
10.4.7 進程退出狀態 466
10.4.8 日誌 467
10.4.9 派生進程 469
10.4.10 向進程傳遞消息 469
10.4.11 進程間信號傳輸 472
10.4.12 控制資源訪問 473
10.4.13 同步操作 474
10.4.14 控制資源的併發訪問 475
10.4.15 管理共用狀態 476
10.4.16 共用命名空間 477
10.4.17 進程池 479
10.4.18 實現MapReduce 480
10.5 asyncio：非同步I/O、事件迴圈和併發工具 484
10.5.1 非同步併發概念 484
10.5.2 利用協程合作完成多工 485
10.5.3 調度常規函式呼叫 488
10.5.4 非同步地生成結果 490
10.5.5 併發地執行任務 492
10.5.6 組合協程和控制結構 495
10.5.7 同步原語 499
10.5.8 提供協定類抽象的非同步I/O 505
10.5.9 使用協程和流的非同步I/O 510
10.5.10 使用SSL 514
10.5.11 與功能變數名稱服務交互 516
10.5.12 使用子進程 518
10.5.13 接收UNIX信號 523
10.5.14 結合使用協程、執行緒與進程 525
10.5.15 用asyncio調試 527
10.6 concurrent.futures：管理併發任務池 530
10.6.1 利用基本執行緒池使用map() 531
10.6.2 調度單個任務 532
10.6.3 按任意順序等待任務 532
10.6.4 Future回檔 533
10.6.5 撤銷任務 534
10.6.6 任務中的異常 535
10.6.7 上下文管理器 536
10.6.8 進程池 537

第 11 章 網路通信 539
11.1 ipaddress：Internet地址 539
11.1.1 地址 539
11.1.2 網路 540
11.1.3 介面 543
11.2 socket：網路通信 544
11.2.1 定址、協議簇和通訊端類型 544
11.2.2 TCP/IP客戶和伺服器 552
11.2.3 使用者資料包客戶和伺服器 558
11.2.4 UNIX域通訊端 560
11.2.5 組播 563
11.2.6 發送二進位資料 566
11.2.7 非阻塞通信和超時 568
11.3 selectors：I/O多工抽象 568
11.3.1 操作模型 569
11.3.2 回送伺服器 569
11.3.3 回送客戶 570
11.3.4 伺服器和客戶 571
11.4 select：高效等待I/O 572
11.4.1 使用select() 572
11.4.2 帶超時的非阻塞I/O 577
11.4.3 使用poll() 579
11.4.4 平臺特定的選項 582
11.5 socketserver：創建網路服務器 583
11.5.1 伺服器類型 583
11.5.2 伺服器物件 583
11.5.3 實現伺服器 584
11.5.4 請求處理器 584
11.5.5 回送示例 584
11.5.6 執行緒和進程 588

第 12 章 互聯網 592
12.1 urllib.parse：分解URL 592
12.1.1 解析 593
12.1.2 反解析 595
12.1.3 連接 596
12.1.4 解碼查詢參數 597
12.2 urllib.request：網路資源訪問 599
12.2.1 HTTP GET 599
12.2.2 編碼參數 600
12.2.3 HTTP POST 601
12.2.4 添加發出首部 602
12.2.5 從請求提交表單數據 602
12.2.6 上傳文件 603
12.2.7 創建定制協議處理器 606
12.3 urllib.robotparser: Internet蜘蛛存取控制 608
12.3.1 robots.txt 608
12.3.2 測試存取權限 609
12.3.3 長壽命蜘蛛 610
12.4 base64：用ASCII編碼二進位資料 611
12.4.1 Base64編碼 611
12.4.2 Base64解碼 612
12.4.3 URL安全的變種 612
12.4.4 其他編碼 613
12.5 http.server：實現Web伺服器的基類 615
12.5.1 HTTP GET 615
12.5.2 HTTP POST 616
12.5.3 執行緒和進程 618
12.5.4 處理錯誤 619
12.5.5 設置首部 620
12.5.6 命令列用法 621
12.6 http.cookies：HTTP cookie 622
12.6.1 創建和設置cookie 622
12.6.2 Morsel 622
12.6.3 編碼的值 624
12.6.4 接收和解析Cookie首部 624
12.6.5 候選輸出格式 625
12.7 webbrowser：顯示Web頁面 626
12.7.1 簡單示例 626
12.7.2 窗口與標籤頁 626
12.7.3 使用特定流覽器 627
12.7.4 BROWSER變數 627
12.7.5 命令列介面 627
12.8 uuid：全域唯一識別碼 628
12.8.1 UUID 1：IEEE 802 MAC地址 628
12.8.2 UUID 3和5：基於名字的值 630
12.8.3 UUID 4：隨機值 631
12.8.4 處理UUID物件 631
12.9 json：JavaScript對象記法 632
12.9.1 編碼和解碼單一資料型別 633
12.9.2 人類可讀和緊湊輸出 633
12.9.3 編碼字典 635
12.9.4 處理定制類型 636
12.9.5 編碼器和解碼器類 638
12.9.6 處理流和文件 640
12.9.7 混合資料流程 641
12.9.8 命令列上處理JSON 641
12.10 xmlrpc.client：XML-RPC的客戶庫 642
12.10.1 連接伺服器 643
12.10.2 資料類型 645
12.10.3 傳遞物件 648
12.10.4 二進位資料 648
12.10.5 異常處理 650
12.10.6 將調用組合在一個消息中 650
12.11 xmlrpc.server：一個XML-RPC伺服器 652
12.11.1 一個簡單的伺服器 652
12.11.2 候選API名 653
12.11.3 加點的API名 654
12.11.4 任意API名 655
12.11.5 公佈物件的方法 656
12.11.6 分派調用 657
12.11.7 自省API 659

第 13 章 email 662
13.1 smtplib：簡單郵件傳輸協定客戶 662
13.1.1 發送email消息 662
13.1.2 認證和加密 663
13.1.3 驗證email地址 666
13.2 smtpd：示例郵件伺服器 667
13.2.1 郵件伺服器基類 667
13.2.2 調試伺服器 669
13.2.3 代理伺服器 670
13.3 mailbox：管理email歸檔 670
13.3.1 mbox 671
13.3.2 Maildir 673
13.3.3 消息標誌 678
13.3.4 其他格式 680
13.4 imaplib：IMAP4客戶庫 680
13.4.1 變種 680
13.4.2 連接伺服器 681
13.4.3 示例配置 682
13.4.4 列出郵箱 682
13.4.5 郵箱狀態 684
13.4.6 選擇郵箱 686
13.4.7 搜索消息 686
13.4.8 搜索規則 687
13.4.9 獲取消息 689
13.4.10 完整消息 693
13.4.11 上傳消息 694
13.4.12 移動和複製消息 695
13.4.13 刪除消息 696

第 14 章 應用構建模組 699
14.1 argparse：命令列選項和參數解析 700
14.1.1 建立解析器 700
14.1.2 定義參數 700
14.1.3 解析命令列 700
14.1.4 簡單示例 701
14.1.5 幫助輸出 707
14.1.6 解析器組織 711
14.1.7 高級參數處理 716
14.2 getopt：命令列選項解析 722
14.2.1 函數參數 722
14.2.2 短格式選項 723
14.2.3 長格式選項 723
14.2.4 一個完整的例子 723
14.2.5 縮寫長格式選項 725
14.2.6 GNU式選項解析 725
14.2.7 結束參數處理 726
14.3 readline：GNU readline庫 727
14.3.1 配置readline 727
14.3.2 完成文本 728
14.3.3 訪問完成緩衝區 731
14.3.4 輸入歷史 733
14.3.5 hook 736
14.4 getpass：安全密碼提示 737
14.4.1 示例 737
14.4.2 無終端使用getpass 738
14.5 cmd：面向行的命令處理器 739
14.5.1 處理命令 739
14.5.2 命令參數 740
14.5.3 現場幫助 741
14.5.4 自動完成 742
14.5.5 覆蓋基類方法 744
14.5.6 通過屬性配置Cmd 745
14.5.7 運行shell命令 746
14.5.8 候選輸入 747
14.5.9 sys.argv的命令 748
14.6 shlex：解析shell類語法 749
14.6.1 解析加引號的字串 749
14.6.2 為shell建立安全的字串 751
14.6.3 嵌入注釋 751
14.6.4 將字串分解為token 752
14.6.5 包含其他token源 752
14.6.6 控制解析器 753
14.6.7 錯誤處理 755
14.6.8 POSIX與非POSIX解析 756
14.7 configparser：處理設定檔 757
14.7.1 設定檔格式 757
14.7.2 讀取設定檔 758
14.7.3 訪問配置設置 759
14.7.4 修改設置 765
14.7.5 保存設定檔 766
14.7.6 選項搜索路徑 767
14.7.7 用拼接合並值 768
14.8 logging：報告狀態、錯誤和資訊消息 772
14.8.1 日誌系統的組成 773
14.8.2 應用與庫中的日誌記錄 773
14.8.3 記入文件 773
14.8.4 旋轉日誌檔 774
14.8.5 詳細級別 774
14.8.6 命名日誌記錄器實例 776
14.8.7 日誌樹 776
14.8.8 與warnings模組集成 777
14.9 fileinput：命令列篩檢程式框架 778
14.9.1 將m3u檔轉換為RSS 778
14.9.2 進度中繼資料 779
14.9.3 原地過濾 781
14.10 atexit：程式關閉回檔 782
14.10.1 註冊退出回檔 782
14.10.2 修飾符語法 783
14.10.3 撤銷回檔 784
14.10.4 什麼情況下不調用atexit函數 785
14.10.5 處理異常 786
14.11 sched：定時事件調度器 787
14.11.1 有延遲地運行事件 788
14.11.2 重疊事件 788
14.11.3 事件優先順序 789
14.11.4 取消事件 790
第 15 章 國際化和當地語系化 791
15.1 gettext：消息編目 791
15.1.1 轉換工作流概述 791
15.1.2 由原始程式碼創建消息編目 792
15.1.3 運行時查找消息編目 794
15.1.4 複數值 795
15.1.5 應用與模組當地語系化 797
15.1.6 切換轉換 798
15.2 locale：文化當地語系化API 798
15.2.1 探查當前當地語系化環境 799
15.2.2 貨幣 803
15.2.3 格式化數位 804
15.2.4 解析數字 805
15.2.5 日期和時間 806
第 16 章 開發工具 807
16.1 pydoc：模組的線上說明 808
16.1.1 純文字幫助 808
16.1.2 HTML幫助 809
16.1.3 互動式幫助 809
16.2 doctest：通過文檔完成測試 810
16.2.1 起步 810
16.2.2 處理不可預測的輸出 811
16.2.3 traceback 814
16.2.4 避開空白符 815
16.2.5 測試位置 819
16.2.6 外部文檔 822
16.2.7 運行測試 824
16.2.8 測試上下文 827
16.3 unittest：自動測試框架 829
16.3.1 基本測試結構 829
16.3.2 運行測試 829
16.3.3 測試結果 830
16.3.4 斷言真值 831
16.3.5 測試相等性 832
16.3.6 幾乎相等？ 833
16.3.7 容器 833
16.3.8 測試異常 837
16.3.9 測試固件 838
16.3.10 用不同輸入重複測試 840
16.3.11 跳過測試 842
16.3.12 忽略失敗測試 842
16.4 trace：執行程式流 843
16.4.1 示例程式 843
16.4.2 跟蹤執行 844
16.4.3 代碼覆蓋 845
16.4.4 調用關係 847
16.4.5 程式設計介面 848
16.4.6 保存結果資料 849
16.4.7 選項 850
16.5 traceback：異常和棧軌跡 850
16.5.1 支援函數 851
16.5.2 檢查棧 851
16.5.3 traceback異常 853
16.5.4 底層異常API 854
16.5.5 底層棧API 857
16.6 cgitb：詳細的traceback報告 859
16.6.1 標準traceback轉儲 859
16.6.2 啟用詳細的traceback 860
16.6.3 traceback中的區域變數 862
16.6.4 異常屬性 864
16.6.5 HTML輸出 866
16.6.6 記錄traceback 866
16.7 pdb：互動式調試工具 868
16.7.1 啟動調試工具 869
16.7.2 控制調試工具 871
16.7.3 中斷點 881
16.7.4 改變執行流 890
16.7.5 用別名定制調試工具 895
16.7.6 保存配置設置 897
16.8 profile和pstats：性能分析 898
16.8.1 運行性能分析工具 898
16.8.2 在上下文中運行 901
16.8.3 pstats：保存和處理統計資訊 901
16.8.4 限制報告內容 903
16.8.5 調用者/被調用者圖 903
16.9 timeit：測量小段Python代碼執行的時間 905
16.9.1 模組內容 905
16.9.2 基本示例 905
16.9.3 將值存儲在字典中 906
16.9.4 從命令列執行 908
16.10 tabnanny：縮進驗證工具 909
16.11 compileall：位元組編譯原始檔案 910
16.11.1 編譯一個目錄 910
16.11.2 忽略文件 911
16.11.3 編譯sys.path 912
16.11.4 編譯單個文件 912
16.11.5 從命令列運行 913
16.12 pyclbr：類流覽器 914
16.12.1 掃描類 915
16.12.2 掃描函數 916
16.13 venv：創建虛擬環境 917
16.13.1 創建環境 917
16.13.2 虛擬環境的內容 917
16.13.3 使用虛擬環境 918
16.14 ensurepip：安裝Python包安裝工具 920

第 17 章 運行時特性 922
17.1 site：全網站配置 922
17.1.1 導入路徑 922
17.1.2 使用者目錄 923
17.1.3 路徑設定檔 924
17.1.4 定制網站配置 926
17.1.5 定制使用者配置 927
17.1.6 禁用site模組 929

17.2 sys：系統特定配置 929
17.2.1 解譯器設置 929
17.2.2 運行時環境 935
17.2.3 記憶體管理和限制 937
17.2.4 異常處理 942
17.2.5 底層執行緒支援 944
17.2.6 模組和導入 947
17.2.7 跟蹤程式運行情況 963

17.3 os：可移植訪問作業系統特定特性 968
17.3.1 檢查檔案系統內容 968
17.3.2 管理檔案系統許可權 971
17.3.3 創建和刪除目錄 973
17.3.4 處理符號連結 973
17.3.5 安全地替換現有檔 974
17.3.6 檢測和改變進程所有者 975
17.3.7 管理進程環境 976
17.3.8 管理進程工作目錄 977
17.3.9 運行外部命令 977
17.3.10 用os.fork()創建進程 979
17.3.11 等待子進程 980
17.3.12 Spawn創建新進程 982
17.3.13 作業系統錯誤碼 982
17.4 platform：系統版本資訊 983
17.4.1 解譯器 983
17.4.2 平臺 984
17.4.3 作業系統和硬體資訊 985
17.4.4 可執行程式體系結構 986
17.5 resource：系統資源管理 987
17.5.1 當前使用情況 987
17.5.2 資源限制 988
17.6 gc：垃圾回收器 990
17.6.1 跟蹤引用 990
17.6.2 強制垃圾回收 992
17.6.3 查找無法回收的物件引用 993
17.6.4 回收閾值和代 995
17.6.5 調試 998
17.7 sysconfig：解譯器編譯時配置 1002
17.7.1 配置變數 1002
17.7.2 安裝路徑 1004
17.7.3 Python版本和平臺 1007


第 18 章 語言工具 1009
18.1 warnings：非致命警告 1009
18.1.1 分類和過濾 1010
18.1.2 生成警告 1010
18.1.3 用模式過濾 1011
18.1.4 重複的警告 1013
18.1.5 候選消息傳送函數 1013
18.1.6 格式化 1014
18.1.7 警告中的棧層次 1014
18.2 abc：抽象基類 1015
18.2.1 ABC如何工作 1015
18.2.2 註冊一個具體類 1016
18.2.3 通過派生實現 1017
18.2.4 輔助基類 1017
18.2.5 不完整的實現 1018
18.2.6 ABC中的具體方法 1019
18.2.7 抽象屬性 1020
18.2.8 抽象類別和靜態方法 1022
18.3 dis：Python位元組碼反彙編工具 1023
18.3.1 基本反彙編 1023
18.3.2 反彙編函數 1024
18.3.3 類 1025
18.3.4 原始程式碼 1026
18.3.5 使用反彙編調試 1027
18.3.6 迴圈的性能分析 1028
18.3.7 編譯器優化 1033
18.4 inspect：檢查現場物件 1035
18.4.1 示例模組 1035
18.4.2 檢查模組 1035
18.4.3 檢查類 1036
18.4.4 檢查實例 1038
18.4.5 文檔串 1038
18.4.6 獲取原始程式碼 1039
18.4.7 方法和函數簽名 1041
18.4.8 類層次體系 1043
18.4.9 方法解析順序 1044
18.4.10 棧與幀 1045
18.4.11 命令列介面 1047

第 19 章 模組和包 1048
19.1 importlib：Python的導入機制 1048
19.1.1 示例包 1048
19.1.2 模組類型 1049
19.1.3 導入模組 1049
19.1.4 載入工具 1051
19.2 pkgutil：包工具 1052
19.2.1 包導入路徑 1052
19.2.2 包的開發版本 1054
19.2.3 用PKG檔管理路徑 1055
19.2.4 嵌套包 1056
19.2.5 包數據 1058
19.3 zipimport：從ZIP歸檔載入Python代碼 1060
19.3.1 示例 1060
19.3.2 查找模組 1061
19.3.3 存取碼 1061
19.3.4 原始程式碼 1062
19.3.5 包 1063
19.3.6 數據 1063
附錄A 移植說明 1066
附錄B 標準庫之外 1081
```

# hashlib函式庫/套件/模組

>* hashlib是python專門提供hash演算法的函式庫，包括md5, sha1, sha224, sha256, sha384, sha512等演算法

```
>>> import hashlib
>>> m = hashlib.md5()
>>> m.update(b"Nobody inspects")
>>> m.update(b" the spammish repetition")
>>> m.digest()
    b'\\xbbd\\x9c\\x83\\xdd\\x1e\\xa5\\xc9\\xd9\\xde\\xc9\\xa1\\x8d\\xf0\\xff\\xe9'

More condensed:
>>> hashlib.sha224(b"Nobody inspects the spammish repetition").hexdigest()
```

##### Python2的範例==>作業:改成Python3
```
import hashlib

data = "I am your greatteacher"
print hashlib.md5(data).hexdigest()
print hashlib.sha1(data).hexdigest()
print hashlib.sha224(data).hexdigest()
print hashlib.sha256(data).hexdigest()
print hashlib.sha384(data).hexdigest()
print hashlib.sha512(data).hexdigest()
```

```
#!/usr/bin/python3
import hashlib
m = hashlib.md5()
data = "I am your greatteacher"

# 先將資料編碼，再更新 MD5 雜湊值
m.update(data.encode("utf-8"))

h = m.hexdigest()
print(h)
```

##### 只是小改變==>答案就會不一樣
```
import hashlib

a = "I am your greatteacher"
print hashlib.md5(a).hexdigest()

b = "I am your ggreatteacher"
print hashlib.md5(b).hexdigest()

c = "I am your Greatteacher"
print hashlib.md5(c).hexdigest()
```

##### 把你的機密檔案Hash
```
#!/usr/bin/env python

import hashlib
import sys

def main():
    if len(sys.argv) != 2:
        sys.exit('Usage: %s file' % sys.argv[0])

    filename = sys.argv[1]
    m = hashlib.md5()
    with open(filename, 'rb') as fp:
        while True:
            blk = fp.read(4096) # 4KB per block
            if not blk: break
            m.update(blk)
    print(m.hexdigest(), filename)

if __name__ == '__main__':
    main()
```
執行看看:

python3 test4.py

python3 test4.py test1.py



## Argparse函式庫/套件/模組

>* https://docs.python.org/3.6/howto/argparse.html
>* https://docs.python.org/2.7/howto/argparse.html

範例:
```
from argparse import ArgumentParser

parser1 = ArgumentParser()
parser2 = ArgumentParser(prog="my_example")
parser3 = ArgumentParser(usage="usage")
parser4 = ArgumentParser(description="a simple demo of argparse")
parser5 = ArgumentParser(epilog="see the doc: https://docs.python.org/3/library/argparse.html")

parser1.print_help()
parser2.print_help()
parser3.print_help()
parser4.print_help()
parser5.print_help()
```
-h 這個選擇性參數 (optional argument) 是自動產生的

##### argparse.ArgumentParser類別
```
class argparse.ArgumentParser(prog=None, usage=None, description=None, epilog=None, parents=[], 
formatter_class=argparse.HelpFormatter, prefix_chars='-', fromfile_prefix_chars=None, argument_default=None, 
conflict_handler='error', add_help=True, allow_abbrev=True)
```
>* Create a new ArgumentParser object. 
>* All parameters should be passed as keyword arguments. 

參數說明
>* prog - The name of the program (default: sys.argv[0])
>* usage - The string describing the program usage (default: generated from arguments added to parser)
>* description - Text to display before the argument help (default: none)
>* epilog - Text to display after the argument help (default: none)
>* parents - A list of ArgumentParser objects whose arguments should also be included
>* formatter_class - A class for customizing the help output
>* prefix_chars - The set of characters that prefix optional arguments (default: ‘-‘)
>* fromfile_prefix_chars - The set of characters that prefix files from which additional arguments should be read (default: None)
>* argument_default - The global default value for arguments (default: None)
>* conflict_handler - The strategy for resolving conflicting optionals (usually unnecessary)
>* add_help - Add a -h/--help option to the parser (default: True)
>* allow_abbrev - Allows long options to be abbreviated if the abbreviation is unambiguous. (default: True)

## 使用 ArgumentParser.add_argument() 加入想解析的參數

參數基本上分兩種，一種是位置參數 (positional argument)，另一種就是選擇性參數 (optional argument)，主要差別在於參數指定方式的不同
>* positional argument ==>根據它出現的位置來指定它的值是多少
>* optional argument 與位置無關，是根據前綴來指定 (底下範例 -o 或 --optional-arg 後面跟著是誰就指定是誰)。
```
from __future__ import print_function
from argparse import ArgumentParser
parser = ArgumentParser()

parser.add_argument("pos1", help="positional argument 1")
parser.add_argument("-o", "--optional-arg", help="optional argument", dest="opt", default="default")

args = parser.parse_args()
print("positional arg:", args.pos1)
print("optional arg:", args.opt)
``` 

執行程式(不帶參數)==>python3 test2.py 

執行畫面
```
usage: test2.py [-h] [-o OPT] pos1
test2.py: error: the following arguments are required: pos1
```

執行程式==>python3 test2.py -h

執行畫面
```
usage: test2.py [-h] [-o OPT] pos1

positional arguments:
  pos1                  positional argument 1

optional arguments:
  -h, --help            show this help message and exit
  -o OPT, --optional-arg OPT
                        optional argument

```

執行程式(帶多個參數)==>python3 test2.py hello 

執行畫面
```
positional arg: hello
optional arg: default
```

執行程式(帶多個參數)==>python3 test2.py hello -o mydeargreatteacher

執行畫面
```
positional arg: hello
optional arg: mydeargreatteacher
```
##### add_argument()函式:
```
ArgumentParser.add_argument(name or flags...[, action][, nargs][, const][, 
default][, type][, choices][, required][, help][, metavar][, dest])
```
>* Define how a single command-line argument should be parsed. 
>* Each parameter has its own more detailed description below, but in short they are:

參數說明
>* name or flags - Either a name or a list of option strings, e.g. foo or -f, --foo.
>* action - The basic type of action to be taken when this argument is encountered at the command line.
>* nargs - The number of command-line arguments that should be consumed.
>* const - A constant value required by some action and nargs selections.
>* default - The value produced if the argument is absent from the command line.
>* type - The type to which the command-line argument should be converted.
>* choices - A container of the allowable values for the argument.
>* required - Whether or not the command-line option may be omitted (optionals only).
>* help - A brief description of what the argument does.
>* metavar - A name for the argument in usage messages.
>* dest - The name of the attribute to be added to the object returned by parse_args().

##### parse_args()函式method的參數:只有兩個參數
```
ArgumentParser.parse_args(args=None, namespace=None)
```
Convert argument strings to objects and assign them as attributes of the namespace. Return the populated namespace.

Previous calls to add_argument() determine exactly what objects are created and how they are assigned. See the documentation for add_argument() for details.

參數說明
>* args - List of strings to parse. The default is taken from sys.argv.
>* namespace - An object to take the attributes. The default is a new empty Namespace object.

# 比較有趣的範例
```
import argparse
parser = argparse.ArgumentParser()
parser.add_argument("square", type=int, help="display a square of a given number")
parser.add_argument("-v", "--verbosity", type=int, help="increase output verbosity")

args = parser.parse_args()

answer = args.square**2

if args.verbosity == 2:
    print("the square of {} equals {}".format(args.square, answer))
elif args.verbosity == 1:
    print ("{}^2 == {}".format(args.square, answer))
else:
    print(answer)
```
```
python3 test3.py 2
4

python3 test3.py 2 -v 1
2^2 == 4

python3 test3.py 2 -v 2
the square of 2 equals 4

python3 test3.py 2 -v 33
答案會是甚麼??
```

#### 作業:將python 2.7的範例改成Python3的範例
https://docs.python.org/2.7/howto/argparse.html
