# file decorators
def fun(fun,val):
    def Fibonacci():
        print("Fibonacci series start printing...")
        n1,n2 = 0,1
        count = 0
        while count < val:
            print(n1,end=" ")
            nth = n1+n2
            n1 = n2
            n2 = nth
            count +=1
        fun()
    return Fibonacci

def done():
    print("\nFibonacci series done")

funused = fun(done,15)
funused()
