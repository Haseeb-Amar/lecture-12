# lecture-12

marks array
#include <array>
#include <string>
#include <algorithm>
using namespace std;
#include <iostream>

int main()
{
    cout << "Hello User!\nEnter marks for five subjects";
    int marks[5];
    int sum=0;
    for (int i = 0; i < 5; i++)
    {
        cout << "\nInput the subject marks" << endl;
        cin >> marks[i];
	//if the user enters alphabet or marks more than 100 or less than zero (negative)
        while (cin.fail() || marks[i]>100 || marks[i]<0) {
            cout << "invalid command, enter the marks again\n";
            cin.clear();
            cin.ignore();
            cin >> marks[i];
        }

          sum = sum + marks[i];
        }
    cout << "\nYour average is: " << sum / 5<<endl;
}
  
months array
  
  #include <iostream>
#include <string>
using namespace std;
int main()
{
    //declaring and initialising string array for the months
    string months[12] = { "January", "February", "March","April","May","June","July","August","September","October","November","December" };
    
    //displaying the values stored in the months array
    for (int i = 0; i < 12; i++)
    {
        cout << months[i] << endl;
    }
}
  
