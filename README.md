# Kitchen-Timetable
for i in range(int(input())):
    n = int(input())
    a = list(map(int, input().split()))
    b = list(map(int, input().split()))
    c = 0
    at = a[0]
    for x in range(0, n):
        if x > 0:
            at = a[x] - a[x-1]
        if at >= b[x]:
            c += 1
    print(c)
