## 期末專案規劃：登山共乘平台

### I. **專案目的**

臺灣大部分登山口都處於大眾交通難以到達的偏遠地區，故坊間山友會在一些平台揪團尋找共乘前往，但是這些未經整理的資訊分布各處，往往需要花費大量時間尋找合適的行程，故希望建立一個以登山健行為主題的共乘資訊平台

想想以資訊的力量解決生活中的問題，幫助有需要的山友們方便搜尋，結識更多志同道合的夥伴。

### II. **產品靈感**

靈感來自於歐洲盛行的共乘平台 ── [BlaBlaCar](https://www.blablacar.co.uk/)，類似搭便車的概念，在網站輸入你要去的地方和預計出發時間，有些會開車經過這些地方的人會把他們的資訊放在上面，你可以搜尋到這些司機的資訊和他們要求攤題的車費，通常都是會比搭巴士更便宜一些（5 歐之類），希望將相同的概念運用在產品上，打造臺灣登山界的 BlaBlaCar，不用再受限於包車或湊不到人而取消行程，也讓一些獨自開車上山的車主願意分享出他們的空位，創造一個能互惠雙方的資訊平台。

最早在 2019 年末，我曾經參加 GDG Taichung 黑客松派對，當時就以這個想法做了一個簡單的 APP，有會員系統、報名機制和行程列表，後來因為活動結束，合作的後端無暇繼續幫忙維護資料、只得擱置完善的想法，不過它可以說是這次計畫的雛型。

![](https://i.imgur.com/G3zE2QC.jpg)

我打算以它為基礎，自己寫後端資料庫及篩選日期的機制，並且加上其他功能，包括第三方登入、登山路線資料的建立、天氣串接及更多細節。

### III. 產品**簡介**

以「登山共乘」為主題的資訊交流平台，訪客可以瀏覽目前最新的共乘貼文，能夠以日期或關鍵字搜尋對應的行程，而註冊並登入後可以發信聯繫車主報名，或選擇開團、成為車主尋找其他乘客，此外，產品將整合 PTT Hiking 版的近期資訊，並且以臉書登入作為驗證，確認用戶真實存在以保障雙方安全性。

### IV. 核心功能

1. 訪客可以瀏覽所有的共乘貼文
    - 日期
    - 登山路線
    - 共乘人數
2. 註冊及登入功能，加入第三方 facebook 登入驗證用戶真實性
3. 登入後
    - 與貼文作者聯繫
    - 新增共乘貼文
    - 收藏共乘貼文
4. 用戶管理後台，可查看、編輯、刪除自身貼文，及記錄收藏或聯繫過的貼文

### V. 待研究的進階功能

- [ ]  建立完整的登山路線資料庫
- [ ]  整合 OSM 地圖資訊，標示登山口或路線位置
- [ ]  整合 Windy API 或 OpenWeatherMap API，以標示該路線近期天氣資訊
- [ ]  未來繼續爬蟲臉書的共乘社團，希望加入更多資訊

---
## User Story

### ****訪客****

- P1 身為訪客，我想在首頁看到所有的共乘貼文
- P1 身為訪客，我希望可以透過日期、山頭或關鍵字篩選，以便尋找適合我的登山行程
- P1 身為訪客，我想聯繫貼文者，因此會進行註冊及登入流程
- P1 身為訪客，我想了解常見問題，幫助快速找到解答
- P1 身為訪客，我想要了解平台的基本資訊
- P2 身為訪客，我希望貼文可以附上入山地點的地圖以便確認登山口位置
- P2 身為訪客，我希望貼文可以附上該路線及天氣狀況，決定是否參與行程
- P2 我希望能夠不登入，就能透過 email 或其他管道聯繫到車主
- P3 我希望有類似山區搜索功能，類似雪山共乘也可以順道載去武陵四秀登山口這種

### 會員

除了以上的訪客功能，身為登入會員

- P1 我希望以第三方進行登入
- P1 我希望可以確認貼文者的真實性
- P1 我可以新增共乘貼文（標題、出發區域、出發日期、內文、人數、路線選擇、共乘費用等）
- P1 我希望可以對我有興趣的貼文寄信給發文者，或取得進一步聯繫
- P1 我希望可以收藏我有興趣的貼文
- P2 我希望新增貼文時可以直接添加資料庫原本存在的路線、登山口
- P2 我希望發布在這邊的資訊能同步產生分享檔案，讓我可以分享在臉書共乘社團或批踢踢
- P2 我希望能有回饋機制，讓彼此能互相評價

### 平台管理者

- P1 我需要瀏覽並管理所有貼文
- P1 我需要瀏覽所有會員
- P1 我希望可以自行新增登山路線，豐富資料庫

---

以上，是目前 side project 雛形