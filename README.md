# -LAB-1--Python-Basics
# Q-1
nums = list(map(int, input("Enter integers: ").split()))
unique_nums = sorted(set(nums), reverse=True)

if len(unique_nums) >= 2:
    print("Second largest unique element:", unique_nums[1])
else:
    print("Not enough unique elements.")

    
    
# Q-2
lst = [10, 20, 10, 30, 20, 40]

result = []
for item in lst:
    if item not in result:
        result.append(item)

print("List after removing duplicates:", result)



# Q-3
nums = list(map(int, input("Enter integers: ").split()))

freq = {}
for num in nums:
    freq[num] = freq.get(num, 0) + 1

for num, count in freq.items():
    print(f"{num}: {count}")
    


   # Q-4
    lst = [10, 20, 30, 40, 50]

rotated = [lst[-1]] + lst[:-1]
print("Rotated list:", rotated)


# Q-5
nums = list(map(int, input("Enter integers: ").split()))
target = int(input("Enter target element: "))

indices = [i for i, x in enumerate(nums) if x == target]
print("Indices:", indices)
