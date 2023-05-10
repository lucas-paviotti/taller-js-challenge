## 1 - Non-Constructible Change

```javascript
const NonConstructibleChange = (coins) => {
   let change = 1;
   const sortedCoins = coins.sort((a, b) => a - b);
   
   for (i = 0; i < sortedCoins.length && sortedCoins[i] <= change; i++) {
      change = change + coins[i];
   }
  
   return change;
}
```

## 2 - Sorted Squared Array

```javascript
const SortedSquareArray = (arr) => arr.map((n) => Math.pow(n, 2)).sort((a, b) => a - b);
```
