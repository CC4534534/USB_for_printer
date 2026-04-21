# USB_for_printer
```
diskpart

list disk

select disk 2         ← 選擇你的隨身碟（號碼請依照 list disk 結果）

clean                 ← ⚠️ 會刪掉所有資料

create partition primary size=32768

select partition 1

active

format fs=fat32 quick

assign letter=E       ← 指定磁碟代號（可改成你想要的）

exit
```
----------------------------
# SD card
diskpart
list disk
select disk 2
clean
convert mbr
create partition primary size=30000
format fs=fat32 quick
assign
exit
