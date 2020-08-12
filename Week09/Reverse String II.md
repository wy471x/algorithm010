## [Reverse String II](https://leetcode.com/problems/reverse-string-ii/description/)

1. > traverse string : 

```java
class Solution {
    public String reverseStr(String s, int k) {
        int len = s.length();
        if (len < k)
            return reverse(s);
        else if (len >= k && len < 2*k) {
            return reverse(s.substring(0, k)) + s.substring(k);
        }

        int count = len / (2 * k), left = len % (2 * k);
        String ans = new String();
        int i = 0;
        while (i < count) {
            ans += reverse(s.substring(i*2*k, i*2*k + k)) + s.substring(i*2*k + k, i*2*k + 2*k);
            i++;
        }

        if (left < k)
            ans += reverse(s.substring(count*2*k));
        else if (left >= k && left < 2*k) {
            ans += reverse(s.substring(count*2*k, count*2*k + k)) + s.substring(count*2*k + k);
        }
        return ans;
    }

    String reverse(String str) {
        char[] ans = str.toCharArray();
        for (int i = 0, j = str.length() - 1; i < j; ++i, --j) {
            char tmp = ans[i];
            ans[i] = ans[j];
            ans[j] = tmp;
        }

        return new String(ans);
    }
}
```

