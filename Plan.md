## Plan entity

### key
namespace: none  
kinds: Plan  
identifiers: auto  
Ancestor paths: [**Company**](https://github.com/bbq-portal-system/BBQ-Database/blob/main/Company.md)  

### properties
```
{
  planName: string,
  planDiscription: string,
  planDetails: [
    {
      menuId: string,
      menuKind: string,
      manuName: string,
      menuCount: int,
      menuUnit: string,
      menuImg: [string, ],  
    },
  ],
  planCost: integer,
  planMinMembers: integer,
  planMaxMembers: integer,
  planReservationNeeds: boolean,
  planImg: [url, ],
}
```

#### planName
```
手ぶら　満腹コース
```
コース名  

**規定値**  
無


#### planDiscription
```
とにかくお得　全員大満足です
```
プラン説明文  

**規定値**  
無


#### planDetails
```
[
  {
    menuId: 'abcd1234',
    menuKind: 'food' or 'drink' or 'tool' or 'others',
    manuName: '特選和牛',
    menuCount: 2,
    menuUnit: 'セット',
    menuImg: ['https://some.jpg', ],  
  },
],
```
メニューの詳細  

**規定値**  
オブジェクトの配列  
＊Name: 名前    
＊Kind: 種類    
＊Count: 数量      
＊Unit: 単位    
＊Discription: 説明文  
＊Img: 画像URLの配列  


#### planCost
```
1800
```
プランの値段（１セット） 

**規定値**　　
半角数字  
```
pattern="(?=.*\d)"
```

#### planMinMembers
```
1
```
プランを注文できる最小数  

**規定値**  
半角数字  
```
pattern="(?=.*\d)"
```

#### planMaxMembers
```
8
```
プランを注文できる最大数 

**規定値**　　
半角数字  
```
pattern="(?=.*\d)"
```


#### planReservationNeeds
```
true
```
事前予約が必要かどうか  

**規定値**　　
Boolean


#### planImg
```
[{url}, {url}, ]
```
プラン内容写真  

**規定値**　　
cloudStorage のURL  



