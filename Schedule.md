## Schedule entity
BBQ会場毎の予約日時を格納します  
主にカレンダーの表示に使用します  

### key
namespace: none  
kinds: Schedule  
identifiers: auto  
Ancestor paths: [**Site**](https://github.com/bbq-portal-system/ER-diagram/blob/main/Site.md)  

### properties
```
{
  year: string,
  month: string,
  date: string,
  time: [string, ],
},
```

#### year
```
'2021'
```
予約年  

**規定値**  
半角数字４桁　文字列  
```
pattern="(?=.*\d).{4,}"
```

#### month
```
'09'
```
予約月  

**規定値**  
半角数字　２桁　文字列  

```
pattern="(?=.*\d).{2,}"
```


#### date
```
'12'
```
予約日 

**規定値**  
半角数字　２桁　文字列  
```
pattern="(?=.*\d).{2,}"
```


#### time
```
['1600', ]
```
予約時間 

**規定値**  
半角数字　４桁　２４時間表示　の配列  
＊利用時間を全部記載
```
pattern="(?=.*\d).{4,}"
```








