def tanh(x):
    e_pos = (2.71828 ** x)
    e_neg = (2.71828 ** -x)
    return (e_pos - e_neg) / (e_pos + e_neg)
i1, i2 = 0.05, 0.10 
w1, w2 = 0.15, 0.20
w3, w4 = 0.25, 0.30
b1 = 0.5
h1 = tanh((i1 * w1) + (i2 * w3) + b1)
h2 = tanh((i1 * w2) + (i2 * w4) + b1)
w5, w6 = 0.40, 0.45
w7, w8 = 0.50, 0.55
b2 = 0.7
o1 = tanh((h1 * w5) + (h2 * w7) + b2)
o2 = tanh((h1 * w6) + (h2 * w8) + b2)
print(" Hidden Layer 1:", h1)
print(" Hidden Layer 2:", h2)
print(" Output Layer 1:", h1)
print(" Output Layer 2:", h2)
