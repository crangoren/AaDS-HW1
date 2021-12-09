Ответы внизу

# AaDS-HW1
homework

1. Прочитать в книге "Грокаем алгоритмы" или в предложенных материалах про алгоритмы и О-большое.
2. Определить сложность следующих алгоритмов:
-. Поиск элемента массива с известным индексом 
-. Дублирование одномерного массива через foreach
-. Удаление элемента массива с известным индексом без сдвига
-. Удаление элемента массива с неизвестным индексом без сдвига
-. Удаление элемента массива с неизвестным индексом со сдвига
.

3. Определить сложность следующих алгоритмов. Сколько произойдет итераций?
a)

        int n = 10000; 
        List<Integer> arrayList = new ArrayList<>();  
        for (int i = 0; i < n; i++) { //n
            for (int j = 1; j < n; j *= 2) { //log n
                arrayList.add(i * j);  //log n
            }
        }
b)

        int n = 10000;
        List<Integer> arrayList = new ArrayList<>();
        for (int i = 0; i < n; i += 2) { logn
            for (int j = i; j < n; j++) { logn
                arrayList.add(i * j); logn
            }
        }
с)

        int n = 10000;
        List<Integer> arrayList = new ArrayList<>();
        for (int i = 0; i < n; i ++) {
            for (int j = 0; j < n; j++) {
                arrayList.add(i * j);
                n--;
            }
        }
d)
```

    factorial(BigInteger.valueOf(10000))

public static BigInteger factorial(BigInteger n) {
    if (n.equals(BigInteger.ONE)) {
        return n;
    }
    return n.multiply(factorial(n.subtract(BigInteger.valueOf(1))));
}

e)
fib(BigInteger.valueOf(50));

public static BigInteger fib(BigInteger n) {
    if (n.equals(BigInteger.ONE)) {
        return BigInteger.ONE;
    }
    if (n.equals(BigInteger.TWO)) {
        return BigInteger.ONE;
    }
    return fib(n.subtract(BigInteger.ONE)).add(fib(n.subtract(BigInteger.TWO)));
}



1) + 

2)
-O(1)
-O(n^2)
-O(1)
-O(n)
-O(n)


3)
a- n^2 или n log n?
b- log n
c- log n
d-
e-
