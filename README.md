# js_code_recipe
jsコードレシピのメモ


```


// 変数宣言
let hoge = 'test';

let myFunction = () => console.log('hoge');

// 定数宣言
const NAME = "なみえ";
NAME = "あむろ"; //エラー

function myFunction(a){
  const result = a+2;
  return result;
}


// アロー関数
関数を簡略化して記述可能
thisを束縛できる

const calcSum = (a,b,c) => {
    const r = a + b + c;
    return r;
}

calcSum(1,2,3);


/* 引数の省略 */
const myFunction = a =>{
    return a+2;
}

// アロー関数の処理が一行の時は{}とreturnを省略できる
const myFunction = (a) => a + 2;


function calc(p, tax = 0.08){
  const r = p + p * tax;
  return r;
}

const result = calc(100);
console.log(result);   // 108


// iphoneかどうかの判定
const isIOs = navigator.userAgent.includes('iphone');
if(isIOs){}



// 配列の扱い
const array = ['鈴木', '佐藤', '高橋'];
console,log(array); // 3



array.forEach((value, index) =>{
    // インデックス
    console.log(index, value);   // 0 イチゴ  1 みかん 2 りんご
});

// forループもかけるよ
for(const value of array){
    console.log(value);  // イチゴ みかん りんご
}


// 人物データを保持したオブジェクト

const person = {
	id : 1,
	name : '鈴木',
	age : 28
	method: () => {
	    console.log('hoeghoeg');
	},
        method2: function(){
	    console.log('hoeghoeg');
	}
}

// objecthはconstで定義しても深い階層はいじれちゃう
// そんな時は 
'use strict'
object.freeze(person);


// 時間差処理
setTimeout( () =>{
	// 何かが起きる
},1000);

setInterval(()=>{
	// 何かが繰り返される
},1000);


btn.addEventListener('click', () =>{
	
});

btn.addEventListener('click', (event) =>{
	
});


// 画面サイズがウインどうを超えた時
const w = matchMedia('(min-width:500px;)');


```
