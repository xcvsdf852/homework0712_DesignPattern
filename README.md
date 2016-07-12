# DesignPattern
<h2>Singleton 獨體模式</h2>
    觀念:
        由類別決定要不要建立物件，資源管理問題，實務上不能有兩個
        用戶端不能建物件，掌控權在類別裡
    
    生活範例:
        加油時，一側的加油島位置和服務員同時只能服務一位客戶加油，
        直到該客戶結束，才能在提供服務給下一位客戶。
        
<h2>Factory 工廠</h2>
    觀念:
        物件透過別人的物件幫忙建立，透過一個類別去建造另一個類別
	    根據傳進來的資料來Nwe相對應的物件
    
    生活範例:
        將炒飯、燴飯、湯、麵功能集合成一家小吃店，告知店員我想要哪個食物物件
        由小吃店根據我開的菜單用判斷的方式提供(new)相對應的物件
        
<h2>FactoryMethod 工廠方法</h2>
    觀念:
        工廠方法把簡單工廠的邏輯判斷一到了用戶端程式法來進行
        
    生活範例:
        將炒飯、燴飯、湯、麵各自建立一個物件，方法名稱相同，但方法內new的物件(飯、麵、湯)不同
        因此在用戶端點菜new炒飯後再執行炒飯裡的方法，就會new實際炒飯物件出來
        
<h2>Prototype 原型模式</h2>
    觀念:
        用原型實例指定建立物件的種類，並且透過拷貝這些原型建立新的物件。
        按照現有的物件再複製一個新的物件，透過__clone() 修改一點不一樣的地方
        從一個物件再建立另外一個可訂製的物件，且不需要知道任何建立的細節。
        
    生活範例:
        打造鑰匙，鑰匙有許多相同的款式，只要大量clone相同款式，
        當要打造符合自己要用的鑰匙時，再根據不同的齒紋修改仿照。
        
<h2>Adapte 轉接器模式</h2>
    觀念:
        A透過B用到C，方法相同但規格不同的
        使原本由於介面不相容而不能一起工作的那些類別可以一起工作
        
    生活範例:
        出國旅遊，不通外語，在短時間內無法加強外語能力前，或改變整個國外說中文時，
        可以找導遊或者翻譯，翻譯的人就是轉接器的一種
        
<h2>Bridge 橋接器</h2>
    觀念:
        與Adapter差異是: Bridge著重介面是標準的但實作方法是分開， Adapter單純轉介
        所以Bridge規格一樣，格式相同，方法不同
        
    生活範例:
        當翻譯精通十多國語言時，在請求協助溝通翻譯時，
        要告知究竟是哪一國語言翻譯成哪一國的語言，或是要去哪一國旅遊
        
<h2>Decorator 裝飾模式</h2>
    觀念:
        包一層上去，包裝上去，又名WRAPPER，當詢問外層和子多少錢時，外層盒子會詢問內部的東西多少錢
    
    生活範例:    
        購買禮物時，增加買外包裝紙，再增加購買包裝紙外的緞帶裝飾，再買個袋子提著，
        透過一層層的統計，就知道禮物+包裝紙+緞帶+提袋的總價值
<h2>Facade 外觀模式</h2>
    觀念:
    	考慮到這個系統不好用所以做個介面操作，固定下來一個方法，讓使用者直操作後面功能
    	而與Adapter差異在於Adapter無法操作，所以弄個轉接介面處理
    	
	生活範例:
	    google 將全世界網站的資訊蒐集起來，做出了一個搜尋介面，根據關鍵字使用規則，從繁雜資訊篩選
	    
<h2>Observer 觀察者模式</h2>
    觀念:
        觀察者模式就是訂閱。
        蒐集一堆訂閱者，當事件發生時觸發，就會將所有的訂閱者執行一遍，
        例如有新電子報時就會將所有訂閱者發送一遍。
        
    生活範例:
        訂購羊奶，業者留下相關資訊，每當早上時，就將羊奶定時定點送得訂購者手中。
        
<h2>Creational  開關</h2>
    觀念:
    	著重互動部分
    	使用者端透過Creational物件 開關  燈泡 電腦 麥克風
    	
    生活範例:	
        透過Creational物件 開關 音響、風扇等
