# Number-of-Good-Pairs-using-Java-Leetcode

    class Solution {
        public int numIdenticalPairs(int[] nums) {
            if(nums.length<1){
                return 0;
            }
            int output = 0;
            for(int i =0;i<nums.length;i++){
                for(int j=i+1;j<nums.length;j++){
                    if(nums[i]==nums[j]){
                        output=output+1;
                    }
                }
            }
            return output;
        }
    }
