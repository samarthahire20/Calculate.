# simple calculator script for the math project
# todo: add error handling for strings later

def do_math(a, b, op):
    # check operation type
    if op == '+' or op == 'add':
        return a + b
        
    elif op == '-' or op == 'sub':
        return a - b
        
    elif op == '*' or op == 'mul':
        return a * b
        
    elif op == '/' or op == 'div':
        if b == 0:
            print("Error: division by zero")
            return None
        return a / b
        
    else:
        print("invalid op")
        return None

# testing it out
print(do_math(10, 5, 'add'))
print(do_math(20, 4, '/'))
