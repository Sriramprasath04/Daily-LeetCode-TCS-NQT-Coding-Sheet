# Complexity
- Time complexity: O(n)
<!-- Add your time complexity here, e.g. $$O(n)$$ -->

- Space complexity: O(1)
<!-- Add your space complexity here, e.g. $$O(n)$$ -->

# Code
```
class Solution {
    static void convertBinaryToDecimal(String num){
        int i = num.length()-1;
        int res = 0;
        int pow = 1;
        while(i >= 0){
            int val = Integer.parseInt(""+num.charAt(i));
            res = res + pow * val;
            System.out.println(""+val+"*"+pow+" = " +res);
            pow = pow * 2;
            i--;
        }
        System.out.println("------");
        System.out.println("Decimal : "+res);
    }
}
```