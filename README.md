# 來自同學的作業

## 第一題

請撰寫一程式，使用者由鍵盤輸入美元金額，輸出兌換的新台幣金額 (假設 1 美元=29.12 台幣)

{% hint style="info" %}
#### 運用概念

此處主要運用的是 **算術運算子**及**輸入輸出**的使用
{% endhint %}

#### C++ 程式範例

```cilkcpp
#include <iostream>

using namespace std;

int main() {
    float USD;
    cout << "請輸入轉換美金金額 (匯率 1 USD = 29.12 TWD): ";
    cin >> USD;

    float TWD = USD * 29.12;
    cout << USD << " USD = " << TWD << " TWD" << endl << "(1 USD = 29.12 TWD)";
}
```

#### 範例輸出

<pre><code><strong>Input:
</strong><strong>請輸入轉換美金金額 (匯率 1 USD = 29.12 TWD): 3
</strong>Output:
3 USD = 87.36 TWD
(1 USD = 29.12 TWD)
</code></pre>



## 第二題

輸入 5 個實數，計算並輸出其平均值

{% hint style="info" %}
#### 運用概念

此處主要運用的是 **算術運算子**及**輸入輸出**的使用
{% endhint %}

{% hint style="info" %}
#### 算術運算子

用於數字上計算的運算子，常用的有下面幾個

\+: 加法

\-: 除法

\*: 乘法

/: 除法

%: 取餘數
{% endhint %}

{% hint style="info" %}
#### 輸入/輸出

常用的輸入輸出方法是 std::cin 及 std::cout，使用方法如下:

#### cin

cin >> variable(一變數)

箭頭記得向內走，越後面的變數越慢拿到數值

如: cin >> A >> B >> C;

則賦值順序為 A -> B -> C

#### cout

cout << variable(一變數)/string(字串)/int(數值)/float(浮點數)

箭頭記得向外走，越後面的資料越晚輸出

如: cout << "今天" << name << "好帥"

就會輸出「今天{name}好帥」(name的內容依變數內容決定)
{% endhint %}

#### C++ 範例程式

```cpp
#include <iostream>

using namespace std;

int main() {
    float A, B, C, D, E;
    cout << "請輸入五個數字 (以空格隔開): ";
    cin >> A >> B >> C >> D >> E;
    cout << "平均值為 " << (A + B + C + D + E) / 5;
}
```

#### 範例輸出如下

<pre><code><strong>Input:
</strong><strong>請輸入五個數字 (以空格隔開): 5 2 1 5 2
</strong>Output:
平均值為 3
</code></pre>

## 第三題

請設計一個程式，可讓使用者輸入一個正整數 n，輸出為 1+2+......+n 的總和
