# leet_code
 explanation :
# Given an arrey [2, 7, 11, 15] and target [target = 9] so that if we add two numbers in the arrey that should be equal to the target 2+7 = 9 and 2 index is 0 and #7 index is 1 [0,1] .
# and should return the indices of that numbers in the arrey [0,1]


from typing import List

class solution:

    def twosum(self, nums : List[int],target:int) :
        num_indices = {}
        print(num_indices)

        for i , num in enumerate(nums):
            # print(i,num)
            complement = target - num 

            if complement  in num_indices:

                return[num_indices[complement],i]
            num_indices[num] =i
            # print(i,num ,"i value ")

nums = [2, 7, 11, 15]
target = 9
solver = solution().twosum(nums, target)
# result = solver.twosum(nums, target)
print("index value of add up numbers ",solver)
# print(result)

