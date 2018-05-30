# HackerRank - [Compare the Triplets](https://www.hackerrank.com/challenges/compare-the-triplets/problem)

완료 코드.

```javascript
function solve(a, b) {
    var result = [];
    var aScore = 0,
        bScore = 0;
    
    for (var i = 0; i < a.length; i++) {
        if (a[i] > b[i]) aScore++;
        if (a[i] < b[i]) bScore++;
    }
    result[0] = aScore;
    result[1] = bScore;
    return result;
}
```

누구는 java 코드로 전부 다 더하는 방식을 취했다. 흠

```java
pointsAlice = ((a0>b0)?1:0)+ ((a1>b1)?1:0)+ ((a2>b2)?1:0) ;
pointsBob = ((a0<b0)?1:0)+ ((a1<b1)?1:0)+ ((a2<b2)?1:0) ;
System.out.println(pointsAlice+" " +pointsBob);
```
