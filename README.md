「莫大毛筆字體」是基於[衡山毛筆フォント](https://opentype.jp/kouzanmouhitufont.htm)的開放原始碼中文字型。衡山毛筆字體是來自於日本書法家青柳衡山，修改前文字＋符號數約：13,000字，修改後文字＋符號數：24,896字，增加11,281字符。

## 字體特色

### 彌補繁體中文常用字缺字缺憾

第一階段的補字已補齊台灣教育部列出的 4,808 個常用字，莫大毛筆字體增加（和修改）168字如下：丢么乒乓俞渝俱值偷偺傻內剁剎剝勻吅叼吆吒吞吳呐呸咚唧唬唳唷啃啕啟啪喱喳喻嗡嗥嗦嗨嗯嘀嘟嘮噓噗噙噥噹嚎嚐囪垮埂塭夠妞姘姬娛婊嫘嬤孓尷巔巢弒彆彞彥徵惦愣懵戶戾拋揄揍揭摹攆晚暨曆术朵查榆檔櫥步歲歷殁每侮毗毽氖氫氯涉唰涮淚渴溉溫溼焊燴狀玨琍產甭盯瞇朧矓矽砸碉稅篡簞粵絕緣罈翱脫腳虛蜕蜢蜥蟑蟬說賒趴跺踩踫蹦塴磞躲鄉醣鈽銬銳錄鍊鎢鎳閱頹颳颼餿骷黃齜

![莫大毛筆字體](https://github.com/max32002/bakudaifont/raw/master/preview/preview.png)

目前新增的字略長，中文字的部份新增6,367字，請參考文字檔 [added_glyph.txt](https://github.com/max32002/bakudaifont/raw/master/added_glyph.txt)。

附註： 由於是「非原作者」的補字，新加入的字在風格上，雖然盡力求一致，難免會與原作者會有一些不同。有一些字補的「超級醜」的，一般情況應該不會遇到，如果有好心人有重做那些醜到爆的字，請再寄給我，感謝。

### 5種字重(Style)

* ExtraLight
* Light
* Regular
* Medium
* Bold

原本的衡山毛筆字體放在Regular 字重 裡，透過程式自動產生ExtraLight、Light、Medium、Bold 新的字重。Light字重是把原本的KouzanBrushFont微微調細一點點。在ExtraLight的字重裡，可能會因為筆劃太細造成某些筆畫消失。在Medium和Bold的字重裡，可能會因為筆劃太粗造成某些筆畫重疊難以識別，有粗體字的需求，可以先挑戰使用Bold字重看看，如果發現效果不如預期，再改用Medium字重。

不能確定自動產生出來的字重裡每一個都是完整的字，畢盡程式會誤判是常有的事情，所以不是在Regular字重裡的筆劃可能會消失。

![莫大毛筆字體](https://github.com/max32002/bakudaifont/raw/master/preview/preview_style.png)

### 清除衡山毛筆字體裡空白的文字

衡山毛筆字體裡有很多空白的字， 會造成無法讓系統自動用預設字體來補字，已清除空白的文字。

### 調整標點符號位置

衡山毛筆字體的全形標點符號針對日本做設計，調整為台灣常見的置中用法。半形的 backslash，調整為非日本地區用法。

### 增加部分臺灣口語、閩南語和客語中文字

例如：喵呣哖唚啥嗍嗝尪䆀掰魩

![莫大毛筆字體臺灣口語字](https://github.com/max32002/bakudaifont/raw/master/preview/preview_taiwaness.png)

### 增加部份的粵語字
感謝網友Luke Liu的貢獻，在莫大毛筆字增加88字如下：㖭㗎乸佢冇冚冧劏叁叻吔吖呔咇咗哋唓唚唞啩啫啱啲啵喺喼嗰嗱嗲嘜嘞嘢嘥嘭噚嚿埗埲塱壆奀嫲嬅孭孻尐戙抆抌拃掹揞揤揼搣搲摙摱摷擝擸攰曱杧氹泵滘瀡烚煲燶甴癦睩瞓矋繑脷膶裇踭躀軚鈪餸𨋢㋿踎

![莫大毛筆字體粵語字](https://github.com/max32002/bakudaifont/raw/master/preview/preview_hk.png)


### 修改
* 原本的衡山毛筆字體「朧」，右邊的龍字有誤，少了三筆劃，已使用其他有筆劃的龍來替代。
* 俞渝偷喻，使用台灣常用的刂，而不是日本常用的《。

## 下載字型

請點選GitHub此畫面右上綠色「Clone or download」按鈕，並選擇「Download ZIP」，或點進想下載的ttf字型檔案，再點「Download」的按鈕進行下載。


## 使用 WebFont

網路字型(Web Font)，用於網頁上的字型顯示，使用者的用戶端不需預先安裝字型檔，一樣能夠看到特殊的字型效果。實現該功能的原理是在瀏覽時才下載字型檔。

可以服用下面的css:
```
@font-face {
  font-family: Bakudai-Regular;
  src: url(https://github.com/max32002/bakudaifont/raw/master/webfont/Bakudai-Regular.woff2) format("woff2")
  , url(https://github.com/max32002/bakudaifont/raw/master/webfont/Bakudai-Regular.woff) format("woff");
}
```
您也可以透過從CDN引入在GitHub上woff2檔案的網址，再把上方的url()內容置換成CDN快取後的網址，將可大幅加快網頁載入。推薦使用 jsDelivr 的服務，在速度上挺不錯的，參考看看： www.cdnperf.com/#!performance,Asia 。

## 附註

* 補的缺字，由於缺乏設計美感，所以效果差強人意，但是聊勝於無。
* 目前是Beta公測版本，歡迎提供測試反饋，請直接反饋在GitHub的Issues中。
* 「偏」字上面沿用日文寫法「戸」，沒有改成台灣用法「戶」，針對「戶」字有另外加字。
* 歡迎一起來補字，如果您也有自己造字並且想更新到莫大毛筆字體裡，請把您的ttf字型檔，透過email(weng.32002@gmail.com)給我，謝謝。由於Max是新手補字，難免補很略醜，如果您也挑戰修改了同一個字，也歡迎寄給我合併，當然您也可以另外再起一個新的字型名稱。

## 著作權與授權

* 本字型是基於改造畫法家青柳衡山先生所開發、發表的「[衡山毛筆フォント](https://opentype.jp/kouzanmouhitufont.htm)」字型。
* 本字型基於 SIL Open Font License 1.1 授權條款免費公開，關於授權合約的內容、免責事項等細節，請詳讀 License 文件。
    * 可自由商用 不需付費、知會或標明作者，即可自由使用此字型，亦可做商業應用。
    * 可自由傳布 可自由分享檔案、將檔案安裝於任何軟硬體中。
    * 可自由改作為其他字型 將字型檔案修改重製為其他字型檔案，改作後的字型檔案須同樣依 Open Font License 釋出。

    
## 相關文章

* 獅尾XD珍珠 Swei.XD.Pearl
https://max-everyday.com/2020/07/swei-xd-pearl/
* 獅尾B2黑體 Swei B2 Sans
https://max-everyday.com/2020/07/swei-b2-sans/
* 獅尾B2宋朝 Swei B2 Serif
https://max-everyday.com/2020/07/swei-b2-serif/
* 獅尾D露西 Swei D Lucy
https://max-everyday.com/2020/07/swei-d-lucy/
* 台灣圓體 TaiwanPearl
https://max-everyday.com/2020/06/taiwanpearl/
* 獅尾肉丸 Swei Meatball
https://max-everyday.com/2020/06/swei-meatball/
* 獅尾四季春字體 Swei Spring
https://max-everyday.com/2020/04/swei-spring/
* 獅尾半月字體 Swei Gothic
https://max-everyday.com/2020/04/swei-half-moon/
* 獅尾圓體 Swei Gothic
https://max-everyday.com/2020/04/swei-gothic/
* 獅尾黑體 Swei Sans
https://max-everyday.com/2020/03/swei-sans/
* 內海字體 (NaikaiFont) 
https://max-everyday.com/2020/03/naikaifont/
* 莫大毛筆字體 (Bakudai)
https://max-everyday.com/2020/03/bakudaifont/
* 正風毛筆字體 (MasaFont)
https://max-everyday.com/2020/05/masafont/
* 清松手寫體 (JasonHandWriting)
https://jasonfonts.max-everyday.com/
* 源泉圓體
https://github.com/ButTaiwan/gensen-font
* jf open 粉圓
https://github.com/justfont/open-huninn-font
* 假粉圓體
https://github.com/max32002/FakePearl
* 俊羽圓體
https://github.com/max32002/YuPearl

## 相關影片
* [MaxCodeReview] FontForge 補缺字：每 (莫大毛筆字體)
https://youtu.be/gGk8b3mkueE
* [MaxCodeReview] FontForge 補缺字：吳 (莫大毛筆字體)
https://youtu.be/AvX97PFLYbM
* [MaxCodeReview] FontForge 補缺字：孓 (莫大毛筆字體)
https://youtu.be/_LXPhFE-VmM
* [MaxCodeReview] FontForge 補缺字：頹 (莫大毛筆字體)
https://youtu.be/4lFKWFG5FE4

## 毛筆字體的應用範例

* 【故宮小劇場】跟著八段錦‧新‧洗武式 https://www.facebook.com/npmshops/posts/3311050418906629


## 贊助Max

很高興可以替中華民國美學盡一分心力，如果你覺得這篇文章寫的很好，想打賞Max，贊助方式如下：
https://max-everyday.com/about/#donate
