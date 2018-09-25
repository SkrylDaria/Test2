string = input()
string = string.lower()
string = string.replace(' ', '')
n = len(string)
i = 0
k = 0
if n % 2 != 0:
    print('NO')
else:
    for i in range(0, n // 2):
        if string[i] == string[n - i - 1]:
            k += 1
        else:
            print('NO')
            break
if k * 2 == n:
    print('YES')
