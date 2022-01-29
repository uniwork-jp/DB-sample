## Reservation entity

### key
namespace: none  
kinds: Reservation  
identifiers: auto  
Ancestor paths: [**Site**](https://github.com/bbq-portal-system/ER-diagram/blob/main/Site.md)  

### properties
```
{
  siteId: string,
  siteName: string,
  orderDate: string,
  reservationDate: string,
  reservationStart: string,
  reservationEnd: string,
  reservationMembers: integer,
  representiveName: string,
  representiveTel: string,
  reservationMenus: [array],
  reservationPlans: [array],
  reservationCost: integer,
  reservationStatus: string,
  reservationNote: string,
  userId: string,
}
```

#### siteId
```
'abcd202'
```
会場ID

**規定値**  
無


#### siteName
```
'淀川河川敷公園枚方地区'
```
会場名  

**規定値**  
無


#### orderDate
```
'20210916'
```
受付日  

**規定値**  
半角数字８桁


#### reservationDate
```
'20210916'
```
予約日  

**規定値**  
半角数字　８桁
```
pattern="(?=.*\d).{8,}"
```


#### reservationStart
```
'1200'
```
開始時間 

**規定値**  
半角数字　４桁　２４時間表示  
```
pattern="(?=.*\d).{4,}"
```


#### reservationEnd
```
'1600'
```
終了時間 

**規定値**  
半角数字　４桁　２４時間表示  
```
pattern="(?=.*\d).{4,}"
```


#### reservationMembers
```
8
```
人数  

**規定値**  
半角数字
```
pattern="(?=.*\d)"
```


#### representiveName
```
'田中　一郎'
```
代表者氏名  

**規定値**  
全角


#### representiveTel
```
'08012345678'
```
代表者電話番号  

**規定値**  
半角数字１１桁　文字列



#### reservationPlans
```
[{planId}, {planId}, ]
```
利用プランの配列  

**規定値**  
planId: string


#### reservationMenus
```
[{menuId}, {menuId}, ]
```
利用メニューの配列  

**規定値**  
menuId: string


#### reservationCost
```
24000
```
予約総額  

**規定値**  
半角数字
```
pattern="(?=.*\d)"
```


#### reservationStatus
```
'orderd'
```
予約状況  

**規定値**  
'ordered': string  
'canceled': string  
'done': string


#### reservationNote
```
備考です
```
追記  

**規定値**  
無


#### userId
```
'some@gmail.com'
```
予約者のユーザーID  

**規定値**  
mailaddress









