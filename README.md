# sitemap產生器
- php do.php [專案網址] [專案名稱]  
- 執行後，會自動在此目錄底下新增[專案目錄]，產生sitemap.txt檔案。

# GA4 Tag 快篩器
- 使用正規表示法篩選，注意結尾要有";"
-       // gtag("參數1","參數2","參數3"); "or' ['|\"]
        // 參數1 ([A-Z|a-z|\d]+)
        // 參數2 ([A-Z|a-z|\d|\-|_]+)
        // 參數3 (\{\s*[^;]+\s*\}) {[不能有;]}
        $pattern = "/gtag\s*\(\s*['|\"]([A-Z|a-z|\d]+)['|\"]\s*,\s*['|\"]([A-Z|a-z|\d|\-|_]+)['|\"]\s*,\s*(\{\s*[^;]+\s*\})\s*\)\s*/";
 