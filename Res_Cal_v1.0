"""
RESISTOR CALCULATOR
A program that calculates the resistor value by inputting its color band

@auth siege
"""

# Define color string list
res_dgt = ['blk', 'brw', 'red', 'ora', 'yel', 'grn', 'blu', 'vio', 'gry', 'wht']
res_mul = ['blk', 'brw', 'red', 'ora', 'yel', 'grn', 'blu', 'vio', 'gry', 'wht', 'gld', 'slv']
res_tol = ['red', 'ora', 'grn', 'blu', 'vio', 'gry', 'gld', 'slv', 'noc']

# Define resistor constants
int_val = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
int_mul = [1e0, 1e1, 1e2, 1e3, 1e4, 1e5, 1e6, 1e7, 1e8, 1e9, 1e-1, 1e-2]
str_tol = ['1%', '2%', '0.50%', '0.25%', '0.10%', '0.05%', '5%', '10%', '20%']

# Input band color
band1 = input("1st Band Color: ")
if band1.lower() in res_dgt:
    index1 = res_dgt.index(band1)
else:
    print("Syntax error")

band2 = input("2nd Band Color: ")
if band2.lower() in res_dgt:
    index2 = res_dgt.index(band2)
else:
    print("Syntax error")

band3 = input("3rd Band Color: ")
if band3.lower() in res_mul:
    index3 = res_mul.index(band3)
else:
    print("Syntax error")

band4 = input("4th Band Color: ")
if band4.lower() in res_tol:
    index4 = res_tol.index(band4)
else:
    print("Syntax error")

print("\nColor Code: {}, {}, {}, {}".format(band1.upper(), band2.upper(), band3.upper(), band4.upper()))

# Math algorithm
dig_conc = ((int_val[index2] * 1) + (int_val[index1] * 10)) * int_mul[index3]
print("Value: {:,} +/- {}".format(dig_conc, str_tol[index4]))
