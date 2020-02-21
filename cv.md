1. Anton Rasoha
2. Telegram @antoshka_rasoha, +375445134294
3. Hmmm, my goals, i really want be confident, that ios developing is my sphere,
   because tried a lot there were not realy intreasting for me. Formula-1 (Ferrari, Sebastian Vettel)
4. C++, C, Python + django, Html, Css
5. ↓↓↓↓↓ footer :)
6. Bsuir labs, some project from it-academy, everything here: https://github.com/WolfandWolf?tab=repositories
7. Bsuir IEF 2y, It-Academy (web developer)
8. Talking with myself, Harry Potter (eng), different films

```
int menu_navigation(int amount_of_func) {                         //function return value of menu point                   
	char word;
	COORD position;
	HANDLE hConsole = GetStdHandle(STD_OUTPUT_HANDLE);
	position.X = 0;
	position.Y = 0;
	SetConsoleCursorPosition(hConsole, position);
	do {
		word = _getch();
		if (word == 80)
			if (position.Y < amount_of_func)
				if (position.Y == amount_of_func - 1) {
					SetConsoleCursorPosition(hConsole, position);
					std::cout << "   " << std::endl;
					position.Y = 0;
					SetConsoleCursorPosition(hConsole, position);
					std::cout << "-> " << std::endl;
				}
				else {
					SetConsoleCursorPosition(hConsole, position);
					std::cout << "   " << std::endl;
					position.Y++;
					SetConsoleCursorPosition(hConsole, position);
					std::cout << "-> " << std::endl;
				}
		if (word == 72)
			if (position.Y > 0) {
				SetConsoleCursorPosition(hConsole, position);
				std::cout << "   " << std::endl;
				position.Y--;
				SetConsoleCursorPosition(hConsole, position);
				std::cout << "-> " << std::endl;
			}
			else {
				SetConsoleCursorPosition(hConsole, position);
				std::cout << "   " << std::endl;
				position.Y = amount_of_func - 1;
				SetConsoleCursorPosition(hConsole, position);
				std::cout << "-> " << std::endl;
			}
		if (word == 13) {
			break;
		}
		if (word == 27)
			return 0;
	} while (1);
	system("cls");
	return position.Y + 1;
}
```
