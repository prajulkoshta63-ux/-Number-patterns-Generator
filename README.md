# -Number-patterns-Generator
print("=="*20)
print(" Number Patterns Generator!")
print("=="*20)

# Right Triangle of Stars
print("=="*20)
print(" Right Triangle of Stars ")
print("=="*20)
rows = 5

for i in range(1, rows + 1):
    for j in range(1, i + 1):
        print("*", end="")
    print()

    #inverted triangle of numbers
print("=="*20)
print(" Inverted Triangle of Numbers ")
print("=="*20)                          
rows = 5
for i in range(rows, 0, -1):
    for j in range(1, i + 1):
        print(j, end="")
    print()

    #Pascal's Triangle
print("=="*20)      
print(" Pascal's Triangle ")                                
print("=="*20)
n = 5
print("\nPascal's Triangle:\n")      
for i in range(n):
    num = 1

    #spaces
    for j in range(n - i -1):
        print(" ", end="")

        #values
        for j in range (i + 1):
            print(num, end=" ")

            # accumulator formula
            num = num * (i-j) // (j + 1)
        print()

#Prime Number up to n 
print("=="*20)
print(" Prime Numbers up to n")                    
print("=="*20)
n = 50
print("\nPrime numbers up to", n, ":\n")
for num in range(2,n + 1):
    for i in range(2, num):
        if num % i == 0:
            break
    else:
        print(num, end=" ")
