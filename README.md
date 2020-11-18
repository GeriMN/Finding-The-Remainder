//Finding The Remainder in C++
#include <iostream>
#include <stdlib.h>
#include <cstdlib>
#include <windows.h>
using namespace std;

void function(int n1, int n2){
    cout << "\n" << "Result: "
         <<n1%n2;
}

int main () {
	
	//the function
	system("Color 70");
    int num1, num2;

    cout << "\nAdd the number: " << flush;
    cin >> num1;

    cout << "\nAdd the other number: " << flush;
    cin >> num2;

	cin.sync();
    function(num1, num2);
    cout << endl;
    
    //the loop
    string response;
    cout << "\n'y' ==> another calculation" << endl;
    cout << "\n'n' ==> quit" << endl;
    cout << endl;
    cin >> response;
    	//if yes
    	system("CLS");
    	for(int i=0;i<=10000;i++) {
    		if (response == "y" || response == "Y") {
    			cout << "\nAdd the number: " << flush;
    			cin >> num1;
    			cout << "\nAdd the other number: " << flush;
    			cin >> num2;
    			function(num1, num2);
    			cout << endl;
    			cout << "\n'y' ==> another calculation" << endl;
    			cout << "\n'n' ==> quit" << endl;
    			cout << endl;
    			cin >> response;
		}
	}
		//if no
	if (response == "n" || response == "N") {
		system("CLS");
		_Exit(0);
	}
		//if invalid response
		for (int j=0;j<=10000;j++) {
			if (response != "n" || response != "N" || response != "y" || response != "Y"){
				system("CLS");
				cout << "\nInvalid response!" << endl;
				cout << "\nTry again: " <<endl;
				cout << endl;
				cin >> response;
				
				
			for(int i=0;i<=10000;i++) {
    			if (response == "y" || response == "Y") {
    				system("CLS");
    				cout << "\nAdd the number: " << flush;
    				cin >> num1;
    				cout << "\nAdd the other number: " << flush;
   					cin >> num2;
   					function(num1, num2);
   					cout << endl;
   					cout << "\n'y' ==> another calculation" << endl;
   					cout << "\n'n' ==> quit" << endl;
   					cout << endl;
   					cin >> response;
    	}
    				if (response == "n" || response == "N"){
    					system("CLS");
    					_Exit(0);
					}
	}
}
}
		//if no
	if (response == "n" || response == "N") {
		_Exit(0);
		}	
return 0;
}
