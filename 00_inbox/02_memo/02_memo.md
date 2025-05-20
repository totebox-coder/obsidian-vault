```dataview
TABLE dateformat(file.ctime, "yyyy-MM-dd[HH:mm]") AS "作成日",
       dateformat(file.mtime, "yyyy-MM-dd[HH:mm]") AS "最終更新日"
FROM "00_inbox/02_memo"
SORT file.ctime DESC
LIMIT 30
```
