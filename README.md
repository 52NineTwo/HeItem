### Matchers(匹配器)
##### .toBe()
相当于```===```比较
```javascript
expect(app).toBe('1'); //app的值是否完全等于1
```
***
##### .toEqual()
相当于```==```比较，注意与```.toBe()```的区别
```javascript
expect(app).toEqual('1');//app的值是否等于1
```
***
##### .toMatch()
按正则表达式进行匹配
```javascript 
expect(app).toMatch(/1/);
```
***
##### .toBeDefined()
检验变量是否定义或赋值
```javascript
var app = '1'
expect(app).toBeDefined(); 检验app是否定义或者赋值
```
##### .toBeNull()
检验变量是否为'null'
