# 99-Bottles-of-Beer
Beginner project: print the lyrics to "99 bottle of beer on the wall."

#include "pch.h"
#include <iostream>
using namespace std;

int main()
{
	for (int bottles = 99; bottles > 0; --bottles) {
		if (bottles == 1) {
			cout << bottles << " bottle of beer on the wall.\n";
			cout << bottles << " bottle of beer\n";
			cout << " Take it down. Pass it around.\n";
			cout << "No more bottles of beer on the wall.\n\n";
		}
		else {
			cout << bottles << " bottles of beer on the wall.\n";
			cout << bottles << " bottles of beer\n";
			cout << " Take one down. Pass it around.\n";
			if (bottles - 1 == 1) {
				cout << bottles - 1 << " bottle of beer on the wall.\n\n";
			}
			else {
				cout << bottles - 1 << " bottles of beer on the wall.\n\n";
			}			
		}		
	}
}
