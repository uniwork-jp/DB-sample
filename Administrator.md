## Administrator entity

### key
namespace: none  
kinds: Administrator  
identifiers: mail address  
Ancestor paths: none  

### properties
```
{
  administratorName: string,
  administratorPassword: string,
  administratorDataPolicy: [array],
  administratorSitePolicy: [array],
}
```

#### administratorName
```
田中　一郎
```
管理者の名前  

**規定値**  
無


#### administratorPassword
```
tana1980
```
パスワード  

**規定値**  
半角英数字　６桁以上　数字、英字の混在必須  
```
pattern="(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{6,}"
```


#### administratorDataPolicy
```
['admin', 'sales', 'reservations']
```
閲覧できる情報の種類  

**規定値**  
'admin', 'sales', 'reservations',いずれか


#### administratorSitePolicy
```
['admin', {siteId}, ]
```
閲覧可能なBBQ会場の種類  

**規定値**　　
admin　全部の会場閲覧可能  
siteId　会場毎に個別

