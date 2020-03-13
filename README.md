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

```
