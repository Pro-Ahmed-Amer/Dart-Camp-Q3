# Dart-Camp-Q3
<u>Assignment - 3</u>

Q \ Separate the **"Even" & "Odd"** numbers between 1-10 in this List 

lst = [1,2,3,4,5,6,7,8,9,10];

using two functions 

1- "myEven(lst)" function to print Even numbers in this list with receive parameter. 

2- "myOdd(lst)" function to print Odd numbers in this list with receive parameter. 

**<u>Notes:</u>**

- Even number => number % 2 = 0
- Odd number => number % 2 = 1

***

1-) Method One :

```dart
main() {
  var lst = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  print('-' * 30);
  myEven(lst);
  print('-' * 30);
  myOdd(lst);
  print('-' * 30);
}

myEven(lst) {
  lst.forEach((element) {
    if (element % 2 == 0) { /* mybe if(element % 2 != 1) */
      print("Even = ${element}");
    }
  });
}

myOdd(lst) {
  lst.forEach((element) {
    if (element % 2 == 1) { /* mybe if(element % 2 != 0) */
      print("Odd = ${element}");
    }
  });
}
```

***

2-) Method Two : 

```dart
main() {
  var lst = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  print('-' * 30);
  myEven(lst);
  print('-' * 30);
  myOdd(lst);
  print('-' * 30);
}

myEven(lst) {
  for (var i = 0; i < lst.length; i++) {
    if (lst[i] % 2 == 0) { /* mybe if(element % 2 != 1) */
      print("Even = ${lst[i]}");
    }
  }
}

myOdd(lst) {
  for (var i = 0; i < lst.length; i++) {
    if (lst[i] % 2 == 1) { /* mybe if(element % 2 != 0) */
      print("Odd = ${lst[i]}");
    }
  }
}
```

***

Output :

```
------------------------------
Even = 2
Even = 4
Even = 6
Even = 8
Even = 10
------------------------------
Odd = 1
Odd = 3
Odd = 5
Odd = 7
Odd = 9
------------------------------
```

