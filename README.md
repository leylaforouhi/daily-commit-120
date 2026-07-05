def find_median(numbers):
    sorted_numbers = sorted(numbers)
    n = len(sorted_numbers)
    middle = n // 2

    if n % 2 == 0:
        return (sorted_numbers[middle - 1] + sorted_numbers[middle]) / 2
    return sorted_numbers[middle]

if __name__ == "__main__":
    values = [8, 3, 5, 12, 7, 9]
    print(f"Values: {values}")
    print(f"Median: {find_median(values)}")
