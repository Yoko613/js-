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
