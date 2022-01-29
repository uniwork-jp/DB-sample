## Menu entity

### key
namespace: none  
kinds: Menu  
identifiers: auto  
Ancestor paths: [**Company**](https://github.com/bbq-portal-system/BBQ-Database/blob/main/Company.md)  

### properties
```
{
  menuName: string,
  menuKind: string,
  menuDiscription: string,
  menuDetails: [
    {
      ingredient: string,
      amount: integer,
      unit: string,
    },
  ],
  menuCost: integer,
  minMembers: integer,
  maxMembers: integer,
  reservationNeeds: boolean,
  menuImg: [url, ],
}
```

#### menuName
```
和牛　リブロース
```
メニュー名  

**規定値**  
無


#### menuKind
```
'food' or 'drink' or 'tool' or 'others'
```
メニュー種類  

**規定値**  
無


#### menuDiscription
```
サシが美しい特上お肉です
```
メニュー説明文  

**規定値**  
無


#### menuDetails
```
 [
    {
      ingredient: '和牛リブロース',
      amount: 100,
      unit: 'g',
      ingredientImg: [url, ],
    },
  ],
```
メニューの詳細  

**規定値**  
オブジェクト  
ingredient: 材料名  
amount: 量  
unit: 単位  
ingredientImg: 材料画像  


#### menuCost
```
1800
```
メニューの値段（１人前） 

**規定値**　　
半角数字  
```
pattern="(?=.*\d)"
```


#### minMembers
```
1
```
メニューを注文できる最小数  

**規定値**  
半角数字  
```
pattern="(?=.*\d)"
```

#### maxMembers
```
8
```
メニューを注文できる最大数 

**規定値**　　
半角数字  
```
pattern="(?=.*\d)"
```


#### reservationNeeds
```
true
```
事前予約が必要かどうか  

**規定値**　　
Boolean


#### menuImg
```
[{url}, {url}, ]
```
メニュー写真  

**規定値**　　
cloudStorage のURL  



