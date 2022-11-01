
m sys import argv

with open(argv[1]) as f:
    for line in f:
        num = int(line)
        print("{:d}=".format(num), end="")
        if num % 2 == 0:
            print("{}*2".format(num//2))
            continue
        for i in range(3, num, 2):
            if num % i == 0:
       
