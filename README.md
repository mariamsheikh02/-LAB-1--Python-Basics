# -LAB-1--Python-Basics
nums = list(map(int, input("Enter integers: ").split()))
unique_nums = sorted(set(nums), reverse=True)

if len(unique_nums) >= 2:
    print("Second largest unique element:", unique_nums[1])
else:
    print("Not enough unique elements.")
