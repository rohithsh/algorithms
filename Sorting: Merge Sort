
def merge_sort(array):
    length = len(array)
    if(length == 1):
        return array
    mp = length//2
    left = array[:mp]
    right = array[mp:]
    left = merge_sort(left)
    right = merge_sort(right)
    return merge(left, right)
    
def merge(left, right):
    result = []
    i = j = 0
    len1 = len(left)
    len2 = len(right)
    while i < len1 and j < len2:
        if left[i] < right [j]:
            result.append(left[i])
            i += 1
        else:
            result.append(right[j])
            j += 1
    
    result.extend(left[i:])
    result.extend(right[j:])
    
    return result

    
array = list(map(int, input().split()))
print(*merge_sort(array), sep = ' ')

    
    
    
