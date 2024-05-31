# contains_dupilcate
class Solution:
   nums = list(map(int,input().split()))
   def containsDuplicate(nums):
       hash_set = set()
        
       for i in nums:
          if i in hash_set:
             return True
          else:
             hash_set.add(i)
       return False
  
   print(containsDuplicate(nums))
