# fibonacci

def fibonacci(x):
    fib = [0,1]
    while fib[-1] < x:
        fib.append(fib[-1] + fib[-2])
    return fib[:-1]
    
x = 4000000
fib_even = [i for i in fibonacci(x) if i%2 ==0]
n = int(input())
print(fib_even[:n])
