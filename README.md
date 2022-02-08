# week-3-c-mode
l <- c(scan())
v <- vector()
n=length(l)
for(i in 1:(n-1)){
  v[i] <- 1
  for(j in (i+1):n){
    if(l[i]==l[j]){
      v[i] <- v[i]+1
    }
  }
}
max <- v[1]
pos <- 1
for(i in 2:n-1)
{
  if(max < v[i]){
    max=v[i]
    pos=i
  }
}
print(l[pos])



OUTPUT:
> l <- c(scan())
1: 5
2: 7
3: 9
4: 6
5: 4
6: 2
7: 3
8: 8
9: 1
10: 2
11: 3
12: 6
13: 4
14: 5
15: 9
16: 5
17: 6
18: 43
19: 599
20: 5
21: 4
22: 3
23: 
Read 22 items
> v <- vector()
> n=length(l)
> for(i in 1:(n-1)){
+   v[i] <- 1
+   for(j in (i+1):n){
+     if(l[i]==l[j]){
+       v[i] <- v[i]+1
+     }
+   }
+ }
> max <- v[1]
> pos <- 1
> for(i in 2:n-1)
+ {
+   if(max < v[i]){
+     max=v[i]
+     pos=i
+   }
+ }
> print(l[pos])
[1] 5
> 
