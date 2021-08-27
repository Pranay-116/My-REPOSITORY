# My-REPOSITORY
SORT AN ARRAY OF 0.'s,1's and 2's DUTCH NATIONAL FLAG
'''void sortColors(vector& nums) {
int low=0;
int mid=0;
int high=nums.size()-1;
while(mid<=high)
{
if(nums[mid]==0){
swap(nums[mid],nums[low]);
low++;
mid++;

        }
        else if(nums[mid]==1)
            mid++;
        else if(nums[mid]==2){
            swap(nums[mid],nums[high]);
            high--;
        }
            
    }
    for(auto it:nums)
        cout<<it<<" ";
    
    
    
}
