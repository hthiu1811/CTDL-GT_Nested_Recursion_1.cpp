# CTDL-GT_Nested_Recursion_1.cpp
Nested Recursion
Nguồn tham khảo : https://codehow.net/de-quy-long-nested-recursion-trong-c-c++-91.html
* Cài đặt :

+ Hàm đệ quy lồng (Nested Recursion) là một hàm đệ quy gọi đối số của nó một đệ quy. 
+ Nghĩa là một hàm mà khi gọi đệ quy, truyền vào tham số chính là hàm đó.

- code : 
int ackerman(int m, int n){
  if(m == 0)
     return n + 1;
  else if(n == 0)
     return ackerman(m - 1, 1);
  else
     return ackerman(m-1, ackerman(m, n-1));
} 
