# Problems-Easy
## Take a list of numbers and display their ranks infront of them

### Answer

      num=[50,100,1,30,76,89,67]

      r=num.copy() #making a copy of our list of numbers
      r.sort() #sorting the copy of our list of numbers

      R=[]  #creating an empty list R
      i=0
      for rank in r:
          rank=i+1
          Rank=[r[i],rank]
          R.append(Rank) #adding the rank of aur sorted list to the empty lisr R

          i=i+1

      for i in range(0,len(num)): #Iterating over the length of list num
          x=0

          if num[i] != R[x][0]:

              while(num[i] != R[x][0]): #while loop used as it will perform the loop till the condition given becomes false
                  x+=1

              print (num[i],',', R[x][1])

          else:
              print (num[i],',', R[x][1])
              
### Output       


    50 , 3
    100 , 7
    1 , 1
    30 , 2
    76 , 5
    89 , 6
    67 , 4
