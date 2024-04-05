# Complexity
- Time complexity: O(n)
<!-- Add your time complexity here, e.g. $$O(n)$$ -->

- Space complexity: O(1)
<!-- Add your space complexity here, e.g. $$O(n)$$ -->

# Code
```
class Solution {
    static void convertDecimalToBinary(int num){
        String res = "";
        while(num>0){
            int digt = num%2;
            res = "" + digt + res;
            num = num/2;
        }

        System.out.println("Result (Decimal to Binary): "+res);
    }
}
```
