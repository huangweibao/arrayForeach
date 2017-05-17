# arrayForeach
数组去重

js 数组去重的方法（人个目前水平认为最优方法）

Array.prototype.unique=function(){
  var newArr = [];
  var obj = [];
  for(var i=0; i<this.length; i++){
    if(!obj[this[i]]){
      newArr.push(this[i]);
      obj[this[i]] = 1;
    }
  }
  return newArr;
}
