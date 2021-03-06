## Вывод программы

    Player A:
    u1 + u2 + u3 + u4 -> min
    12u1 + 16u3 + 19u4 >= 1
    6u1 + 5u2 + 19u3 + 12u4 >= 1
    3u1 + 16u2 + 12u3 + 7u4 >= 1
    17u1 + 18u3 + 2u4 >= 1
    9u1 + 15u2 + 11u3 + 13u4 >= 1
    Initial table:
    +---------+-------------+-------------+-------------+-------------+-------------+
    |    C    |           1 |           0 |           0 |           0 |           0 |
    +---------+-------------+-------------+-------------+-------------+-------------+
    |  basis  |          u1 |          u5 |          u8 |          u9 |           b |
    |   u4    |     -28/155 |      -9/155 |       8/155 |           0 |       1/155 |
    |   u6    |    4838/465 |    -161/465 |    -253/465 |        -1/3 |     104/465 |
    |   u7    |  18827/2325 |    931/2325 |   -862/2325 |      -16/15 |     86/2325 |
    |   u3    |     299/310 |       1/155 |     -19/310 |           0 |      17/310 |
    |   u2    |    229/4650 |    106/2325 |      1/4650 |       -1/15 |     97/4650 |
    +---------+-------------+-------------+-------------+-------------+-------------+
    |    W    |   -388/2325 |    -14/2325 |    -22/2325 |       -1/15 |    191/2325 |
    +---------+-------------+-------------+-------------+-------------+-------------+

    Iteration 1
    +---------+-------------+-------------+-------------+-------------+-------------+
    |    C    |           1 |           0 |           0 |           0 |           0 |
    +---------+-------------+-------------+-------------+-------------+-------------+
    |  basis  |          u1 |          u5 |          u8 |          u9 |           b |
    |   u4    |     -28/155 |      -9/155 |       8/155 |           0 |       1/155 |
    |   u6    |    4838/465 |    -161/465 |    -253/465 |        -1/3 |     104/465 |
    |   u7    |  18827/2325 |    931/2325 |   -862/2325 |      -16/15 |     86/2325 |
    |   u3    |     299/310 |       1/155 |     -19/310 |           0 |      17/310 |
    |   u2    |    229/4650 |    106/2325 |      1/4650 |       -1/15 |     97/4650 |
    +---------+-------------+-------------+-------------+-------------+-------------+
    |    W    |   -388/2325 |    -14/2325 |    -22/2325 |       -1/15 |    191/2325 |
    +---------+-------------+-------------+-------------+-------------+-------------+
    u: [ 0 97/4650 17/310 1/155 ], W: 191/2325
    u1: 0, x1: 0
    u2: 97/4650, x2: 97/382
    u3: 17/310, x3: 255/382
    u4: 1/155, x4: 15/191
    W: 191/2325, g: 2325/191


    Player B:
    v1 + v2 + v3 + v4 + v5 -> max
    12v1 + 6v2 + 3v3 + 17v4 + 9v5 <= 1
    5v2 + 16v3 + 15v5 <= 1
    16v1 + 19v2 + 12v3 + 18v4 + 11v5 <= 1
    19v1 + 12v2 + 7v3 + 2v4 + 13v5 <= 1
    Initial table:
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |    C    |           1 |           1 |           1 |           1 |           1 |           0 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |  basis  |          v1 |          v2 |          v3 |          v4 |          v5 |           b |
    |   v6    |          12 |           6 |           3 |          17 |           9 |           1 |
    |   v7    |           0 |           5 |          16 |           0 |          15 |           1 |
    |   v8    |          16 |          19 |          12 |          18 |          11 |           1 |
    |   v9    |          19 |          12 |           7 |           2 |          13 |           1 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |    Z    |          -1 |          -1 |          -1 |          -1 |          -1 |           0 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+

    Iteration 1
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |    C    |           1 |           1 |           1 |           1 |           1 |           0 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |  basis  |          v1 |          v2 |          v3 |          v4 |          v5 |           b |
    |   v6    |          12 |           6 |           3 |          17 |           9 |           1 |
    |   v7    |           0 |           5 |          16 |           0 |          15 |           1 |
    |   v8    |          16 |          19 |          12 |          18 |          11 |           1 |
    |   v9    |          19 |          12 |           7 |           2 |          13 |           1 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |    Z    |          -1 |          -1 |          -1 |          -1 |          -1 |           0 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+

    Iteration 2
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |    C    |           1 |           1 |           1 |           1 |           0 |           0 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |  basis  |          v2 |          v3 |          v4 |          v5 |          v9 |           b |
    |   v6    |      -30/19 |      -27/19 |      299/19 |       15/19 |      -12/19 |        7/19 |
    |   v7    |           5 |          16 |           0 |          15 |           0 |           1 |
    |   v8    |      169/19 |      116/19 |      310/19 |        1/19 |      -16/19 |        3/19 |
    |   v1    |       12/19 |        7/19 |        2/19 |       13/19 |        1/19 |        1/19 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |    Z    |       -7/19 |      -12/19 |      -17/19 |       -6/19 |        1/19 |        1/19 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+

    Iteration 3
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |    C    |           1 |           1 |           1 |           0 |           0 |           0 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |  basis  |          v2 |          v3 |          v5 |          v8 |          v9 |           b |
    |   v6    |   -3149/310 |   -1133/155 |     229/310 |    -299/310 |      28/155 |      67/310 |
    |   v7    |           5 |          16 |          15 |           0 |           0 |           1 |
    |   v4    |     169/310 |      58/155 |       1/310 |      19/310 |      -8/155 |       3/310 |
    |   v1    |      89/155 |      51/155 |     106/155 |      -1/155 |       9/155 |       8/155 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |    Z    |      37/310 |     -46/155 |     -97/310 |      17/310 |       1/155 |      19/310 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+

    Iteration 4
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |    C    |           1 |           1 |           0 |           0 |           0 |           0 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |  basis  |          v2 |          v3 |          v7 |          v8 |          v9 |           b |
    |   v6    |   -4838/465 | -18827/2325 |   -229/4650 |    -299/310 |      28/155 |    388/2325 |
    |   v5    |         1/3 |       16/15 |        1/15 |           0 |           0 |        1/15 |
    |   v4    |     253/465 |    862/2325 |     -1/4650 |      19/310 |      -8/155 |     22/2325 |
    |   v1    |     161/465 |   -931/2325 |   -106/2325 |      -1/155 |       9/155 |     14/2325 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    |    Z    |     104/465 |     86/2325 |     97/4650 |      17/310 |       1/155 |    191/2325 |
    +---------+-------------+-------------+-------------+-------------+-------------+-------------+
    v: [ 14/2325 0 0 22/2325 1/15 ], Z: 191/2325
    v1: 14/2325, x1: 14/191
    v2: 0, x2: 0
    v3: 0, x3: 0
    v4: 22/2325, x4: 22/191
    v5: 1/15, x5: 155/191
    Z: 191/2325, h: 2325/191
