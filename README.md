//Primitive Quiz

#include <string>   
#include <iostream>
#include <math.h>
using namespace std;

int main() {

	string capital;
	cout << "What is the capital of France: ";
	cin >> capital;
	if (capital == "paris" || capital == "Paris")
	{
		cout << "\nYour answer " << capital << " is correct!" << endl;
	}
	else
	{
		cout << "\nYour answer " << capital << " is incorrect!" << endl;
	}

	return 0;
}
  
//Letter Checker
 #include <string>   
#include <iostream>
#include <math.h>
using namespace std;

int main() {

	char l;
	char L[10] = { 'a', 'e', 'i', 'o', 'u','A', 'E', 'I', 'O', 'U' };
	cout << "Letter Checkerinator, Please Enter a letter: ";
	cin >> l;

	if (!isalpha(l)) {
		cout << l << " is a special character\n";
		return 0;
	}
	for (int i = 0; i < 11; i++) {
		if (l == L[i]) {
			cout << '\n' << l << " is a vowel\n";
			break;
		}
		else {
			cout << '\n' << l << " is a consonant\n";
			break;
		}
	}
	return 0;
}

//Mark My Words
#include <iostream>
using namespace std;
int main()
{	
	while (1)
	{
		cout << "Grading System Inator\n\n";
		double grade;
		cout << "Input the grade of the student out of 100\n\n";
		cin >> grade;
		if (grade < 40)
		{
			cout << "\nGive the student a F\n\n";
		}
		else if (grade >= 40 && grade <= 49)
		{
			cout << "\nGive the student a D\n\n";
		}
		else if (grade >= 50 && grade <= 59)
		{
			cout << "\nGive the student a C\n\n";
		}
		else if (grade >= 60 && grade <= 69)
		{
			cout << "\nGive the student a B\n\n";
		}
		else if (grade >= 70)
		{
			cout << "\nGive the student an A\n\n";
		}
	}
}
//Starting a Band

#include <iostream>
#include <string>
using namespace std;
int main()
{
	bool musicalFriend;
	cout << "Hey friend! if you play an instrument press 1 if not press 0\n\n";
	cin >> musicalFriend;
	if (musicalFriend)
	{
		string friendPlays = "guitar";
		string whatdoesfriendplay;
		cout << "\nWhat instrument do you play\n\n";
		cin >> whatdoesfriendplay;
		if (friendPlays==whatdoesfriendplay)
		{
			cout << "\nNoice you're in we have a gig tonight\n\n";
		}
		else
		{
			cout << "\nYou ain't my friend no more get out of here!\n\n";
		}
	}
	else
	{
		cout << "\nWhy are you even here?\n\n";
	}


}

//Killing Time

#include <iostream>
#include <string>
using namespace std;
int main()
{
	cout << "What to do when waiting for a friend\n\n";
	int x;
	cout << "Type how many minutes longer will your friend take to arive\n\n";
	cin >> x;
	if (x>=15)
	{
		cout << "\nYou're friend will arive 15 or more minutes later what do you want to do?\n\n";
		double c;
		cout << "How much money do you have?\n\n";
		cin >> c;
		if (c>=5)
		{
			cout << "\nGo buy a coffee while waiting for your friend who is always late and you shouldnt tolerate that\n\n";
		}
		else
		{
			cout << "\nGo for a walk and contemplate why you're still friends with someone who doesn't value your time\n\n";
		}
	}
	else
	{
		cout << "\nThis guy is a good friend he'll be here in less than 15 minutes just sit in the food court and wait but,\nyou will be hungry because you will smell all the food\n\n";
	}
}

//Earthquake

#include <iostream>
using namespace std;
int main()
{	
	cout << "MagnitudeInator for earthquakes\n\n";
	cout << "is there an earthquake? Type Yes or No only\n\n";
	string x;
	cin >> x;
	if (x == "yes" || x == "Yes")
	{		
			cout << "\nWhat is the magnitude of the earthquake?\n\n";
			double magnitude;
			cin >> magnitude;
			if (magnitude < 2)
			{
				cout << "\nThis is only a micro earthquake stay calm\n\n";
			}
			else if (magnitude >= 2 && magnitude <= 3)
			{
				cout << "\nThis earthquake is not that bad its very minor be calm\n\n";
			}
			else if (magnitude >= 3 && magnitude <= 4)
			{
				cout << "\nThis earthquake is minor but stay indoors and avoid windows just incase\n\n";
			}
			else if (magnitude >= 4 && magnitude <= 5)
			{
				cout << "\nThis is a light earthquake find shelter\n\n";
			}
			else if (magnitude >= 5 && magnitude <= 6)
			{
				cout << "\nThis is a Moderate earthquake!! if you are outdoors find open ground and stay low avoid buildings\n\n";
			}
			else if (magnitude >= 6 && magnitude <= 7)
			{
				cout << "\nThis Earthquake is a Strong earthquake find something solid like a table and go under it, if you are outdoors find open ground\n\n";
			}
			else if (magnitude >= 7 && magnitude <= 8)
			{
				cout << "\nThis is a Major Earthquake!! say your prayers\n\n";
			}
			else if (magnitude >= 8 && magnitude <= 10)
			{
				cout << "\nThis is a Great earthquake there's not much to do anymore but pray\n\n";
			}
			else if (magnitude > 10)
			{
				cout << "\nHave you watched the movie 2012? yeah this is it, you gonna die, there is no hope, Goodbye :)\n This is a Meteoric Earthquake\n\n";
			}		
	}
	else
	{
		cout << "\nThere is no Earthquake chill\n\n";
	}
}
