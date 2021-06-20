# Dynamic-char


#include<iostream>
using namespace std;
int main()
{
	char* str = new char[255];
	cin >> str;
	for (int i = 0; i < strlen(str); i++)
	{
		if (str[i] == '(')
		{
			int j = i + 1;
			while (str[j] != ')')
			{
				cout << str[j++];
			}
			cout << endl;
		}
	}
	return 0;
}
