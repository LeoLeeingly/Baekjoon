w,h,n = map(int,input().split())
a = list(map(int,input().split()))
cnt = w * h
for i in range(1,n):
    whole = w * h
    w = w // 2
    h = h // 2
    if w * h > a[i]:
        cnt += a[i] + (w*h - a[i])*4
        a[i-1] -= (w*h - a[i])*4
    else:
        cnt += w * h
    if a[i-1] < whole - w*h*4:
        print(-1)
        exit()
    else:
        cnt -= w * h * 4
print(cnt)
