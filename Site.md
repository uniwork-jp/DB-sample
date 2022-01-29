## Site entity

### key
namespace: none  
kinds: Site  
identifiers: auto  
Ancestor paths: none  

### properties
```
{
  siteName: string,
  siteCompany: string,
  siteDiscription: string,
  siteRegion: string,
  sitePrefecture: string,
  siteDistrict: string,
  siteArea: string,
  siteZipcode: string,
  siteAddress: string,
  siteTel: string,
  sitePlans: [array],
  siteMenus: [array],
  siteConditions: [array],
  siteOpen: string,
  siteClose: string,
  siteHoliday: {
    inWeek: [string, ],
    byDate: [string, ],
  },
  siteStation: string,
  siteGeo: geoPointValue: obj,
  siteNote: string,
  siteImg: [string, ],
}
```

#### siteName
```
淀川河川敷公園
```
BBQ会場名  

**規定値**  
無


#### siteCompany
```
株式会社　Est
```
会場運営会社  

**規定値**  
無


#### siteDiscription
```
お花畑が美しい会場です
```
会場紹介文  

**規定値**  
無


#### siteRegion
```
関西
```
地方名  

**規定値**  
無



#### sitePrefecture
```
大阪
```
都道府県  

**規定値**  
無


#### siteDistrict
```
淀川
```
区、大地域  

**規定値**  
無


#### siteArea
```
枚方
```
小地域  

**規定値**  
無


#### siteZipcode
```
'5660054'
```
BBQ会場の郵便番号  

**規定値**  
半角数字　７桁　文字列 


#### siteAddress
```
'大阪府摂津市鳥飼八防1-20-17'
```
BBQ会場の住所  

**規定値**　　
無


#### siteTel
```
'08012345678'
```
BBQ会場の郵便番号  

**規定値**  
半角数字　１１桁  文字列


#### sitePlans
```
[{planId}, {planId}, ]
```
BBQ会場で提供可能なプランの種類  

**規定値**　　
planId　プラン毎に個別設定


#### siteMenus
```
[{menuId}, {menuId}, ]
```
BBQ会場で提供可能なメニューの種類  

**規定値**　　
menuId　メニュー毎に個別設定


#### siteConditions
```
[{conditionId}, ]
```
利用可能なBBQ会場の施設  

**規定値**　　
environmentKey　施設ごとに設定



#### siteOpen
```
'1200'
```
BBQ会場の開場時間  

**規定値**  
半角数字　４桁　２４時間表示  文字列  


#### siteClose
```
'1800'
```
BBQ会場の閉場時間  

**規定値**  
半角数字　４桁　２４時間表示　文字列  


#### siteHoliday
```
{
  inWeek: [string, ],
  byDate: [string, ],
},
```
BBQ会場の休日設定  

**規定値**　　
inWeek: 'sanday', 曜日を配列内に格納  
byDate: '1231', 休日を半角４桁（文字列）で配列内に格納


#### siteStation
```
大阪モノレール　南摂津駅
```
BBQ会場最寄りの駅  

**規定値**　　
無


#### siteGeo
```
{
  "latitude": number,
  "longitude": number
}
```
BBQ会場のジオタグ  

**規定値**　　
オブジェクト


#### siteNote
```
備考
```
BBQ会場の備考欄  

**規定値**　　
無


#### siteImg
```
[
  'https://www.google.com/img.jpg',
]
```
画像のURL配列  
GoogleStorageのアドレス  

**規定値**　　
無



