# 6/14 課題 学んだ記録

自身が学んだ記録を作りましょう。

- 関数(`function` で始まるコード)は全て function.js に書きます
- その他をREADME.md（このファイル）に書いていきます
    - 書き方は README-example.md (同じフォルダに同梱) を参考にしてください
- 書き方は自身でアレンジしてもかまいません


--------------------------------------

## 授業スライドの説明（4時間目～5時間目）

説明の中で実行したログ、分かったこと、疑問などがあればここに書く。

### Consoleの実行ログ
function um(){
  var total = 0;
  for (var counter = 1; counter <= 10; counter++){
	total += counter;
  }

  window.alert(total);
}
undefined
sum();
VM240:1 Uncaught ReferenceError: sum is not defined
    at <anonymous>:1:1
(anonymous) @ VM240:1
function um(rangeTo){
  var total = 0;
  for (var counter = 1; counter <= rangeTo; counter++){
	total += counter;
  }

  window.alert(total);
}
undefined
function um(rangeTo){
  var total = 0;
  for (var counter = 1; counter <= rangeTo; counter++){
	total += counter;
  }

  window.alert(total);
}
undefined
function sum(rangeTo){
  var total = 0;
  for (var counter = 1; counter <= rangeTo; counter++){
	total += counter;
  }

  window.alert(total);
}
undefined
function sum(rangeTo,rangeto){
  var total = 0;
  for (var counter = rangeFrom; counter <= rangeTo; counter++){
	total += counter;
  }

  window.alert(total);
}
undefined
sum(1,10);
VM280:3 Uncaught ReferenceError: rangeFrom is not defined
    at sum (<anonymous>:3:22)
    at <anonymous>:1:1
sum @ VM280:3
(anonymous) @ VM290:1
sum(2, 5);
VM280:3 Uncaught ReferenceError: rangeFrom is not defined
    at sum (<anonymous>:3:22)
    at <anonymous>:1:1
sum @ VM280:3
(anonymous) @ VM291:1
var total = 0;
for (var counter = rangeFrom; counter <= rangeTo; counter++) {
  if (counter % 2 !=1){
    continue;
  }
total += counter;
 }


total;
VM431:2 Uncaught ReferenceError: rangeFrom is not defined
    at <anonymous>:2:20
(anonymous) @ VM431:2
var total = 0;
for (var counter = rangeFrom; counter <= rangeTo; counter++) {

total += counter;
 }


window.alert(total);
VM512:2 Uncaught ReferenceError: rangeFrom is not defined
    at <anonymous>:2:20
(anonymous) @ VM512:2
function sum(rangeFrom,rangeTo){

VM535:1 Uncaught SyntaxError: Unexpected end of input
function sum(rangeTo,rangeFrom = 1){
  var total = 0;
  for (var counter = rangeFrom; counter <= rangeTo; counter++){
	total += counter;
  }

  window.alert(total);
}
undefined
sum(10);
undefined
total
0
total;
0
var hoge = 5;
function testScope(){
  window.alert(hoge);
}
undefined
testScope();
undefined
function sum(rangeTo,rangeFrom = 1){
  var total = 0;
  for (var counter = rangeFrom; counter <= rangeTo; counter++){
	total += counter;
  }

  window.alert(total);
}
undefined
sum(1,10);
undefined
sum(1,10);
undefined
function sum(rangeTo,rangeFrom = 1){
  let total = 0;
  for (let counter = rangeFrom; counter <= rangeTo; counter++){
	total += counter;
  }

  window.alert(total);
}
undefined
sum(1,10);
undefined
function sum(rangeTo,rangeFrom = 1){
  let total = 0;
  for (let counter = rangeFrom; counter <= rangeTo; counter++){
	total += counter;
  }

  window.alert(counter);
}
undefined
sum(1,10);
undefined
function sum(rangeTo,rangeFrom = 1){
  var total = 0;
  for (var counter = rangeFrom; counter <= rangeTo; counter++){
	total += counter;
  }

  if (withDialog){
  window.alert(total);
}
VM767:9 Uncaught SyntaxError: Unexpected end of input
function sum(rangeTo,rangeFrom = 1){
  var total = 0;
  for (var counter = rangeFrom; counter <= rangeTo; counter++){
	total += counter;
  }

  if (withDialog){window.alert(total);
}
VM798:8 Uncaught SyntaxError: Unexpected end of input
function sum(rangeTo,rangeFrom = 1){
  var total = 0;
  for (var counter = rangeFrom; counter <= rangeTo; counter++){
	total += counter;
  }

   if (withDialog)
	 {window.alert(total);
 }else{
  console.log(total);
 }
}
undefined
var total = 0;
function sum(rangeFrom,rangeTo);{
  for (var counter = rangeFrom; counter <= rangeTo; counter++){
	total +=counter;

  }
}
VM980:2 Uncaught SyntaxError: Unexpected token ;
var total = 0;
function sum(rangeFrom,rangeTo){
  for (var counter = rangeFrom; counter <= rangeTo; counter++){
	total +=counter;

  }
}
undefined
sum(1,10);
undefined
window.alert(total);
undefined
sum(1,10);
undefined
window.alert(total);
undefined
function isNarrow((){
  return window.innerWidth < 1000;
}
VM1104:1 Uncaught SyntaxError: Unexpected token (
function isNarrow(){
  return window.innerWidth < 1000;
}
undefined
if (isNarrow()){
	window.alert('狭いです')
}else{
 window.alert('広いです');
}
undefined
```
//[配列]
【var sampleArray = [];
undefined
sampleArray;
[]
var sampleArray = [];
undefined
sampleArray.push(59);
1
sampleArray;
[59]
sampleArray.push(59);
2
sampleArray;
(2) [59, 59]
function calculateTaxIncluding((prices){
	var results = [];
	for (varindex = 0, length = prices.length; index < length; index++)
    {
		results.push(prices[index] * 1.08);
    }
	return results;
}
VM1442:1 Uncaught SyntaxError: Unexpected token (
function calculateTaxIncluding(prices){
	var results = [];
	for (varindex = 0, length = prices.length; index < length; index++)
    {
		results.push(prices[index] * 1.08);
    }
	return results;
}
undefined
calculateTaxIncluding([100,200,40,50]);
VM1443:3 Uncaught ReferenceError: index is not defined
    at calculateTaxIncluding (<anonymous>:3:45)
    at <anonymous>:1:1
calculateTaxIncluding @ VM1443:3
(anonymous) @ VM1471:1
function calculateTaxIncluding(prices){
	var results = [];
	for (var index = 0, length = prices.length; index < length; index++)
    {
		results.push(prices[index] * 1.08);
    }
	return results;
}
undefined
calculateTaxIncluding([100,200,40,50]);
(4) [108, 216, 43.2, 54]
var a = [0,1,1,2,3,5,8];
undefined
a.join(' and ');
"0 and 1 and 1 and 2 and 3 and 5 and 8"
var a = [0,1,1,2,3,5,8];
undefined
a.join();
"0,1,1,2,3,5,8"
var a = [0,1,1,2,3,5,8];
undefined
a.indexOf(5);
5
a.indexOf(4);
-1
a.indexOf(1);
1
a.lastindexOf(1);
VM1548:1 Uncaught TypeError: a.lastindexOf is not a function
    at <anonymous>:1:3
(anonymous) @ VM1548:1
a.lastIndexOf(1);
2】
```

### Console以外の動き（もしあれば）

【ここに書く（なければ省略可）】

### 分かったこと

【ここに書く】

### 疑問・分からないこと（もしあれば）

【ここに書く（なければ省略可）】

--------------------------------------

以下、教科書の自分で読んだ・実行した箇所について書く。

## 4-x ○○ (p.xx)

### Consoleの実行ログ

```
【ここに書く】
```

### Console以外の動き（もしあれば）

【ここに書く（なければ省略可）】

### 分かったこと

【ここに書く】

### 疑問・分からないこと（もしあれば）

【ここに書く（なければ省略可）】
