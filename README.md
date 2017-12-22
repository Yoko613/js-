# js-深意
## 判断一个对象属性是本身还是继承而来

   var modle = {
      name: 'liuc',
      age: '25'
  }
  
 ### 判断继承而来的对象
     'name' in model   true 
     'toString' in model true
     
### 判断不是继承而来
    modle.hasOwnProperty('name')   true 
    modle.hasOwnProperty('toString')  false
    
## js 对 0 , undefine , null ,NAN  默认都是false  。其他默认 ture 
     var aa = 'abcd';
     if (aa.length) {
     }

## 高阶函数-filter 
      var arr = [1,2,4,5,7,9];
      arr.filter(function (x) {return x%2 !== 0})
      [1, 3, 5, 7, 9]
