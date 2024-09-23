#Merge Sorting in simple Concept:

def merge_sort(arr):
    # Checking whether the length of the array is greater than 1.
    # If it's not, there's no need to sort, as an array of length 1 or 0 is already sorted.
    if len(arr) > 1:
        
        # Dividing the array into two halves by finding the middle index.
        mid = len(arr) // 2
        
        # Creating the left part of the array, which consists of elements from the start to the middle.
        left_arr = arr[:mid]
        
        # Creating the right part of the array, which consists of elements from the middle to the end.
        right_arr = arr[mid:]
    
        # Recursively sorting the left half. This will keep dividing until arrays of length 1 are reached.
        merge_sort(left_arr)
        
        # Recursively sorting the right half.
        merge_sort(right_arr)
        
        # Initializing pointers i, j, k to 0.
        # i will be used to track the current index of the left array,
        # j for the right array, and k for the position in the original array.
        i = j = k = 0
        
        # Comparing elements from the left and right arrays and merging them back into the original array.
        while i < len(left_arr) and j < len(right_arr):
            # If the current element in the left array is smaller, place it in the original array.
            if left_arr[i] < right_arr[j]:
                arr[k] = left_arr[i]
                i += 1  # Move the pointer in the left array forward.
            else:
                arr[k] = right_arr[j]  # Otherwise, place the element from the right array.
                j += 1  # Move the pointer in the right array forward.
            k += 1  # Move the pointer in the original array forward.
        
        # If there are remaining elements in the left array, add them to the original array.
        while i < len(left_arr):
            arr[k] = left_arr[i]
            i += 1
            k += 1
        
        # If there are remaining elements in the right array, add them to the original array.
        while j < len(right_arr):
            arr[k] = right_arr[j]
            j += 1
            k += 1


# Test the merge_sort function
arr = [2, 7, 4, 5, 6, 8, 3, 1]
merge_sort(arr)
print(arr)  # Output: [1, 2, 3, 4, 5, 6, 7, 8]
