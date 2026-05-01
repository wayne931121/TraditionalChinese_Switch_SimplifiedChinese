# TraditionalChinese_Switch_SimplifiedChinese
 Traditional Chinese 2 Simplified Chinese, Simplified Chinese 2  Traditional Chinese.

# Models

https://github.com/wayne931121/-TraditionalChinese_Switch_SimplifiedChinese/releases

# Code
```js
let data;
async function sc2tcload(filename='sc2tc.json') {
    const response = await fetch(filename);
    data = await response.json();
    str = "雨落下的那个夜晚，我还傻傻站在那里";
    res = ""    
    for(let c=0;c<str.length;c++){
            res+=data[str.substring(c,c+1)];
    }
    console.log(res);
}
sc2tcload()
```

```js
let data;
async function tc2scload(filename='tc2sc.json') {
    const response = await fetch(filename);
    data = await response.json();
    str = "雨落下的那個夜晚，我還傻傻站在那裡";
    res = ""    
    for(let c=0;c<str.length;c++){
            res+=data[str.substring(c,c+1)];
    }
    console.log(res);
}
tc2scload()
```
