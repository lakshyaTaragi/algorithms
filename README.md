# Algorithms

## BubbleSort
Bubble sort compares each pair of elements in a list and swaps them if they are out of order until the list is sorted.
### Visual
![Bubble sorting](bubbleSort/bubbleSort.gif)

### Code:
```javascript
function bubbleSort(arr) {
    var done = false;
  
    while(!done){
      done = true;
        for (var i = 0; i < arr.length - 1; i++) {
            if (arr[i] > arr[i+1]) {
                var temp = arr[i];
                arr[i] = arr[i+1];
                arr[i+1] = temp;
                done = false;
            }
        }
    }
    return arr;
}

bubbleSort([2, 6, 1, 9, 3, 8, 5, 4, 7]);
```
