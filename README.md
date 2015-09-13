# -WSQ06-Random-number


#include iostream
#include ctime
using namespace std;

int main(void)

{

     int iNumber;
     int iUserguess;
     int iGuesses = 0;

    while(true)
    {
           system("CLS");
           cin.clear();
           iGuesses = 0;

    srand(static_cast<unsigned int>(time(0)));
    iNumbers = rand()%1000+1;
    cout << "Guess the number" << endl;
    do
    {
        cout << "Enter your guess: ";
    cin>> iUserguess;
    if(iUserguess > iNumber)
    {
                  cout << "Too High!" << endl << endl;
    }
    if(iUserguess > iNumber)
    {
                  cout << "Too Low!" << endl << endl;
    }
    iGuesses ++;
    
}while(iUserguess > iNumber || iUserguess < iNumber);

cout << "You guessed the right number! High Five!" << endl << endl;

cout << "You took" << iGuesses << " guesses" << endl << endl;

system("PAUSE");

}

return 0;
