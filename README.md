# Remove-duplicates-from-sorted-array
class Solution {
    public int removeDuplicates(int[] nums) {
        int n = nums.length;
        if (n == 0) return 0;
        int[] temp = new int[n];
        int k = 0;
        for (int i = 0; i < n; i++) {
            boolean found = false;
            for (int j = 0; j < k; j++) {
                if (temp[j] == nums[i]) {
                    found = true;
                    break;
                }
            }
            if (!found) {
                temp[k] = nums[i];
                k++;
            }
        }
        for (int i = 0; i < k; i++) {
            nums[i] = temp[i];
        }
        return k;
    }
}
