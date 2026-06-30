# Remove-duplicates-from-sorted-array
Brute force Approach
Create an empty temporary array.
For every number in the original array:
    Check if it already exists in the temporary array.
    If it exists:
        Ignore it.
    Otherwise:
        Add it to the temporary array.
Copy the temporary array back to the original array.
Return the number of unique elements.
