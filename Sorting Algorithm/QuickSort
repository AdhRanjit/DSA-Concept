#Explanation:
'''
In quicksort algorithm, initialize one random data(middle preferable)
then arrange them either left or right depending after the comparision
and do the recursio

'''
def quick_sort(arr):
    if len(arr) <= 1:
        return arr
    else:
        pivot = arr[len(arr) // 2]
        left = [x for x in arr if x < pivot]
        middle = [x for x in arr if x == pivot]
        right = [x for x in arr if x > pivot]
        
        return quick_sort(left) + middle + quick_sort(right)

arr = [1,3,5,2,6,4]
arranged = quick_sort(arr)
print(arranged)
