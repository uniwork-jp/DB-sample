## User entity

### key
namespace: none  
kinds: User  
identifiers: **mail address**  
Ancestor paths: none  

### properties
```
{
  userName: string,
  userTel: integer,
  userPassword: string,
}
```

#### userName
```
田中　一郎
```
会員の名前  

**規定値**  
無


#### userTel
```
'08012345678'
```
会員の電話番号  

**規定値**  
数字１１桁　文字列


#### userPassword
```
tana1980
```
パスワード  

**規定値**  
半角英数数字　６桁以上　数字、英字の混在必須  
```
pattern="(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{6,}"
```







