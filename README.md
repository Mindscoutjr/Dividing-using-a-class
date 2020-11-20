#include <iostream>

using namespace std;

class item {
    int a, b;
  public:
    void set_values (int,int);
    int area() {return a/b;}
};

void item::set_values (int x, int y) {
  a = x;
  b = y;
}

int main () {
  item quotient;
  quotient.set_values (8,4);
  cout << "quotient: " << quotient.area();
  return 0;
}
