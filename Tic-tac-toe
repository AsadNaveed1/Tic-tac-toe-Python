size = int(input('Size--> '))

ls1 = list(range(0, size ** 2))
lf= []
win= False
winX= False
winO= False
for i in range(0, len(ls1), size):
    gap= 1
    ls2 = []
    for x in range(i, i + size):
        if gap< size:
            print(f"{ls1[x]:>2}", end=' ')
            ls2.append(ls1[x])
            gap+=1
        else:
            print(f"{ls1[x]:>2}", end='')
            ls2.append(ls1[x])
    print()
    lf += [ls2]
while win == False:
    player1= int(input("X--> "))
    ls1[player1] = "X"

    lf= []
    for i in range(0, len(ls1), size):
        gap = 1
        ls2 = []
        for x in range(i, i + size):
            if gap < size:
                print(f"{ls1[x]:>2}", end=' ')
                ls2.append(ls1[x])
                gap += 1
            else:
                print(f"{ls1[x]:>2}", end='')
                ls2.append(ls1[x])
        print()
        lf += [ls2]
        #for row
    for c in range (size):
        countX= 0
        countO= 0
        for h in lf[c]:
            if h== "X":
                countX+=1
                if countX == size:
                    winX = True
            elif h== "O":
                countO+=1
                if countO == size:
                    winO= True
        # for coloumn
    for t in range(size):
        colcountX=0
        colcountO=0
        for i in range(size):
            if lf[i][t]== "X":
                colcountX +=1
                if colcountX == size:
                    winX = True
            elif lf[i][t]== "O":
                colcountO +=1
                if colcountO== size:
                    winO= True


    for y in range(size):
        drcountX=0
        drcountO=0
        for i in range(0,(((size-1)*(size+1))+1),size+1):
            if ls1[i] == "X":
                drcountX+=1
                if drcountX == size:
                    winX = True
            elif ls1[i]== "O":
                drcountO+=1
                if drcountO == size:
                    winO = True

    for y in range(size):
        dlcountX=0
        dlcountO=0
        for i in range((size-1),(((size-1)*size)+1),(size-1)):
            if ls1[i] == "X":
                dlcountX+=1
                if dlcountX == size:
                    winX = True
            elif ls1[i]== "O":
                dlcountO+=1
                if dlcountO == size:
                    winO = True

    if winX== True:
        print("Winner: X")
        win= True
        break

    elif winO== True:
        print("Winner: O")
        win= True
        break


    else:
        count=0
        for j in range(size):
            for t in range(size):
                if lf[j][t]== "X" or lf[j][t]== "O":
                    count+=1
        if count == size**2:
            print("None")
            win= True
            break


    player2= int(input("O--> "))
    ls1[player2] = "O"
    lf=[]
    for i in range(0, len(ls1), size):
        gap = 1
        ls2 = []
        for x in range(i, i + size):
            if gap < size:
                print(f"{ls1[x]:>2}", end=' ')
                ls2.append(ls1[x])
                gap += 1
            else:
                print(f"{ls1[x]:>2}", end='')
                ls2.append(ls1[x])

        print()
        lf += [ls2]
    for c in range (size):
        cntX= 0
        cntO= 0
        for h in lf[c]:
            if h== "X":
                cntX+=1
                if cntX == size:
                    winX = True
            elif h== "O":
                cntO+=1
                if cntO == size:
                    winO= True

    for t in range(size):
        colcountX=0
        colcountO=0
        for i in range(size):
            if lf[i][t]== "X":
                colcountX +=1
                if colcountX == size:
                    winX = True
            elif lf[i][t]== "O":
                colcountO +=1
                if colcountO== size:
                    winO= True


    for y in range(size):
        drcountX=0
        drcountO=0
        for i in range(0,(((size-1)*(size+1))+1),size+1):
            if ls1[i] == "X":
                drcountX+=1
                if drcountX == size:
                    winX = True
            elif ls1[i]== "O":
                drcountO+=1
                if drcountO == size:
                    winO = True

    for y in range(size):
        dlcountX=0
        dlcountO=0
        for i in range((size-1),(((size-1)*size)+1),(size-1)):
            if ls1[i] == "X":
                dlcountX+=1
                if dlcountX == size:
                    winX = True
            elif ls1[i]== "O":
                dlcountO+=1
                if dlcountO == size:
                    winO = True

    if winX== True:
        print("Winner: X")
        win= True
        break

    elif winO== True:
        print("Winner: O")
        win= True
        break


    else:
        count=0
        for j in range(size):
            for t in range(size):
                if lf[j][t]== "X" or lf[j][t]== "O":
                    count+=1
        if count == size**2:
            print("None")
            win= True
            break

    if (winX and winO== False):
        continue
