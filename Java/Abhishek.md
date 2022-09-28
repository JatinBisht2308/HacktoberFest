#Here is a function to find the peak element in an array
public int findPeakElement(int[] nums) {
int[] arr = new int[nums.length];
for(int i =0;i<nums.length;i++){
arr[i]=nums[i];
}
Arrays.sort(arr);
for(int i =0;i<nums.length;i++){
if(nums[i]==arr[nums.length-1]){
return i;
}
}
return -1;
}
