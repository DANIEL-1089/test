#include <iostream>
#include <cstdlib>
#include <ctime>
#include <wchar.h>
#include <Windows.h>
#include <algorithm>
#include <vector>
#include <string>

using namespace std;
Class critter { 
Public:
Critter(int hung);
Void enter() ;
Private:
Int* m_hunger;
}
Critter::Critter(int hung){
m_hunger = new int(hung);
} 
Void critter::enter() {
Cout << "my hunger is: " << *m_hunger << endl; 


int main()
{
    
    Critter* crit1 = new Critter(4);
    Crit1.enter()

    return 0;
}
