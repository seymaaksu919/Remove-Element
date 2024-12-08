class Solution {
    public int removeElement(int[] nums, int val) {
        int k = 0;
        for(int  i= 0; i< nums.length; i++){
            if(nums[i]!= val) {
                nums[k] = nums[i];
                k++;
            }
        }
        return k;
    }

 public static void main(String[] args) {
Solution solution = new Solution();
int [] nums = {2,2,3,4,5,5};
int val = 2;
    System.out.println(solution.removeElement(nums,val));
    }
}
