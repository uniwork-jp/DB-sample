## Tool entity

### key
namespace: none  
kinds: Tool  
identifiers: auto  
Ancestor paths: none  

### properties
```
{
  toolName: string,
  toolDiscription: 
  toolDetails: [
    {
      ingredient: string,
      amount: integer,
      unit: string,
      ingredientImg: [url, ],
    },
  ],
  toolCost: integer,
  toolMinMembers: integer,
  tolMaxMembers: integer,
  toolReservationNeeds: boolean,
  toolImg: [url, ],
}
```

#### toolName
```
大型テント
```
設備名  

**規定値**  
無


#### toolDiscription
```
開放型屋外用テントです
```
メニュー説明文  

**規定値**  
無


#### toolDetails
```
 [
    {
      toolDetailName: '和牛リブロース',
      toolDetailAmount: 1,
      toolDetailUnit: '張',
      toolDetailImg: ['https:some.png', ],
    },
  ],
```
メニューの詳細  

**規定値**  
オブジェクト  
toolDetailName: 単一設備名  
toolDetailAmount: 量  
toolDetailUnit: 単位  
toolDetailImg: 設備画像配列　GoogleCloudStorageのURL  


#### toolCost
```
1800
```
設備の値段（１人前） 

**規定値**　　
半角数字  
```
pattern="(?=.*\d)"
```


#### toolMinMembers
```
1
```
メニューを注文できる最小数  

**規定値**  
半角数字  
```
pattern="(?=.*\d)"
```

#### toolMaxMembers
```
8
```
メニューを注文できる最大数 

**規定値**　　
半角数字  
```
pattern="(?=.*\d)"
```


#### toolReservationNeeds
```
true
```
事前予約が必要かどうか  

**規定値**　　
Boolean


#### toolImg
```
['https:some.png', ]
```
設備写真  

**規定値**　　
cloudStorage のURL  



