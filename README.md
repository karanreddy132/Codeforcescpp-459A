# Codeforcescpp-459A
#include <bits/stdc++.h>

using namespace std;

int main(){
  int x1,y1,x2,y2;
  cin >> x1 >> y1 >> x2 >> y2;

  int sid_lenx = abs(x1-x2);
  int sid_leny = abs(y1-y2);

  if(x1==x2 || y1==y2){
    cout << x1+sid_leny << " " << y1+sid_lenx << " " << x2+sid_leny << " " << y2+sid_lenx;
  }
  else if(abs(x1-x2)==abs(y1-y2)){
    cout << x1 << " " << y2 << " " << x2 << " " << y1;
  }
  else{
    cout << -1;
  }
  return 0;
}
