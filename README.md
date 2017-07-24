## Matchers(匹配器)
>在任何Matcher(匹配器)前加上```not```代表相反的意思(```expect(app).not.toEqual(1) //app的值不等于1```)
### .toBe()
相当于```===```比较
```javascript
expect(app).toBe('1'); //app的值是否完全等于1
```
***
### .toEqual()
相当于```==```比较，注意与```.toBe()```的区别
```javascript
expect(app).toEqual('1');//app的值是否等于1
```
***
### .toMatch()
按正则表达式进行匹配
```javascript 
expect(app).toMatch(/1/);
```
***
### .toBeDefined()
检验变量是否定义或赋值
```javascript
var app = '1';
expect(app).toBeDefined(); //检验app是否定义或者赋值
```
***
### .toBeNull()
检验是否为```null```
```javascript
var app = null;
expect(app).toBenull(); //检验app是否为'null', Success
```
***
### .toBeTruthy()
如果转换为布尔值，是否为```true```
```javascript
expect({}).toBeTruthy();
```
***
### .toBeFalsy()
如果转换为布尔值，是否为```false```
```javascript
expect('').toBeFalsy();
```
***
### .toContain()
数组中是否包含某个元素(值)，只能用于数组，不能用于对象。
```javascript
expect([1,9,9,7]).toContain(9);  //数组中存在9,Success
```
***
### .toBeLessThan()
数值比较 < 小于。检查变量是否小于某个数字
```javascript
var app = '2';
expect(app).toBeLessThan(10); //app的值小于10,Success
```
***
### .toBeGreaterThan()
数值比较 > 大于。检查变量是否大于某个数字
```javascript
var app = '9';
expect(app).toBeGreaterThan(2); //app的值大于2,Success
```
***
### .toBeCloseTo()
