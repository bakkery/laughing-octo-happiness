# H1 Header Size



![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)

array_string = input("Give me your array.\n")
array_given = array_string.strip("[").strip("]").split(", ")

num1 = input("What number would you like to test?\n")
index_given = array_given.index(num1)

i = 1
while True:
    if array_given [-1] == num1:
        print("true")
        if array_given[index_given - i] > num1:
            print(f"Larger number {array_given[index_given - i]} found closer at lower index, {index_given - i}")
        break
    else:
        if index_given - i > i and array_given[index_given + i] > num1 and array_given[index_given - i] > num1:
            print(f"It's a tie! Larger number {array_given[index_given + i]} found {i} numbers away at indices {index_given - i}\
                AND {index_given + i}")
            break
        elif array_given[index_given + i] > num1:
            print(f"Larger number {array_given[index_given + i]} found closer at higher index, {index_given + i}")
            break
        elif index_given - i > -1 and array_given[index_given - i] > num1:
            print(f"Larger number {array_given[index_given - i]} found closer at lower index, {index_given - i}")
            break
    i += 1
    
