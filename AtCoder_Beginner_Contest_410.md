---
title: AtCoder Beginner Contest 410 
categories: 算法题解
description: 我好菜啊
tags:
  - AtCoder
date: 2025-06-22 23:50:08

---


<details>
  <summary>省流版</summary>


- A.模拟
- B. <++>
- C. <++>
- D. <++>
- E. <++>
- F. <++>
- G. <++>

</details>
<br>

## [A - G1 (abc410 A)](https://atcoder.jp/contests/abc410/tasks/abc410_a)

### 题目大意

输入n个数字和一个k，并且计算当中大于等于k的数字个数并且输出

### 解题思路

很简单的一个模拟

<details>
  <summary>神奇的代码</summary>


```cpp
#include<bits/stdc++.h>
using namespace std;
void solve(){
    int n,k,cnt = 0;
    vector<int>a;
    cin >> n;
    for(int i= 1;i <= n;i ++){
        int x;cin >> x;
        a.push_back(x);
    }
    cin >> k;
    for(int i = 0;i < n;i ++){
        if(a[i] >= k)cnt ++;
    }
    cout << cnt;
}

int main(){
    int n = 1;
   //cin >> n;
    while(n --){
        solve();
    }
    return 0;
}
```

</details>
<br>

***

## [B - Reverse Proxy (abc410 B)](https://atcoder.jp/contests/abc410/tasks/abc410_b)

### 题目大意

给定n个空箱子，有q个球，还有一个长度为q的序列X,对于$$X_i$$如果大于等于1，就把球放在$$X_i$$位置上，如果为0，就把球放在拥有最小球的数量的最靠前的箱子里，每次操作输出球放置的箱号

### 解题思路

模拟

<details>
  <summary>神奇的代码</summary>


```cpp
#include<bits/stdc++.h>
using namespace std;

void solve(){
    int n,q;
    cin >> n >> q;
    int x[q],box[n];
    memset(box,0,sizeof box);
    for(int i = 1;i <= q;i ++){
        cin >> x[i - 1];
    }
    for(int i = 0;i < q;i ++){
        if(x[i] == 0){
            int pos = -1,minn = 1e9;
            for(int i = 0;i < n;i ++){
                if(box[i] < minn){
                    minn = box[i];
                    pos = i + 1;
                }
            }
            box[pos - 1] ++;
            cout << pos << ' ';
        }
        else{
            box[x[i] - 1] ++;
            cout << x[i] << ' ';
        }
    }
}

int main(){
    int n = 1;
   //cin >> n;
    while(n --){
        solve();
    }
    return 0;
}
```

</details>
<br>

***

## [C - Rotatable Array (abc410 C)](https://atcoder.jp/contests/abc410/tasks/abc410_c)

### 题目大意

<++>

### 解题思路

<++>

<details>
  <summary>神奇的代码</summary>


```cpp

```

</details>
<br>

***

## [D - XOR Shortest Walk (abc410 D)](https://atcoder.jp/contests/abc410/tasks/abc410_d)

### 题目大意

<++>

### 解题思路

<++>

<details>
  <summary>神奇的代码</summary>


```cpp

```

</details>
<br>

***

## [E - Battles in a Row (abc410 E)](https://atcoder.jp/contests/abc410/tasks/abc410_e)

### 题目大意

<++>

### 解题思路

<++>

<details>
  <summary>神奇的代码</summary>


```cpp

```

</details>
<br>

***

## [F - Balanced Rectangles (abc410 F)](https://atcoder.jp/contests/abc410/tasks/abc410_f)

### 题目大意

<++>

### 解题思路

<++>

<details>
  <summary>神奇的代码</summary>


```cpp

```

</details>
<br>

***

## [G - Longest Chord Chain (abc410 G)](https://atcoder.jp/contests/abc410/tasks/abc410_g)

### 题目大意

<++>

### 解题思路

<++>

<details>
  <summary>神奇的代码</summary>


```cpp

```

</details>
<br>

***
