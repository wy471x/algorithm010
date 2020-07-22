## [旋转数组的最小数字]( https://leetcode-cn.com/problems/xuan-zhuan-shu-zu-de-zui-xiao-shu-zi-lcof/ )

1. > BF : time = O(n) space = O(1)

```java
class Solution {
    public int minArray(int[] numbers) {
        int len = numbers.length;
        int min = numbers[0];
        for (int i = 1; i < len; ++i) {
            if (numbers[i] < min)
                min = numbers[i];
        }
        return min;
    }
}
```

2. > binary search : time = O(logn) space = O(1)

```java
class Solution {
    public int findMin(int[] nums) {
        int low = 0, high = nums.length - 1;
        while (low < high) {
            int mid = low + (high - low) / 2;
            if (nums[mid] > nums[high]) {
                low = mid + 1;
            } else if (nums[mid] < nums[high]) {
                high = mid;
            } else {
                high -= 1;
            }
        }
        return nums[high];
    }
}
```

