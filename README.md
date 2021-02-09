# Fibonacci-Sum-of-Even
Question: By Project Euler:
Each new term in the Fibonacci sequence is generated by adding the previous two terms. By starting with 1 and 2, the first 10 terms will be:
1, 2, 3, 5, 8, 13, 21, 34, 55, 89, ...
By considering the terms in the Fibonacci sequence whose values do not exceed four million, find the sum of the even-valued terms.


c = 33

def fib(number_of_terms):

    counter = 0
    first = 0
    second = 1
    temp = 0
    b = 0
    while counter <= number_of_terms:
        #print(first)
        temp = first + second
        first = second
        second = temp
        counter = counter + 1

        if first %2 ==0:
            b += first
        if counter == c:
            print(b)
fib(c)
