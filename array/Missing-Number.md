<!-- 268. Missing Number -->

<!-- Given an array nums containing n distinct numbers in the range [0, n], return the only number in the range that is missing from the array. -->

code:-

class Solution {
public:
    int missingNumber(vector<int>& nums) {
        int sum1=0;
        int sum2=0;
        for(int i=1;i<=nums.size();i++)
        {
            sum1+=i;
        }
        for(int i=0;i<nums.size();i++)
        {
            sum2+=nums[i];
        }

        return sum1-sum2;
    }
};