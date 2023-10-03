#include <iostream>
#include <cstdlib>
#include <ctime>
#include <wchar.h>
#include <Windows.h>
#include <algorithm>
#include <vector>
#include <string>

using namespace std;
class Critter {
public:
    Critter(int hung);
    void enter();
private:
    int* m_hunger;
};
Critter::Critter(int hung) {
    m_hunger = new int(hung);
}
void Critter::enter() {
    cout << "my hunger is: " << *m_hunger << endl;
} 


int main()
{
    setlocale(LC_ALL, "ru");
    
    Critter* crit1 = new Critter(4);
    crit1->enter();

    return 0;
}
