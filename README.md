# DIT1253-2
Programming assignment 2. DEADLINE 25-10-2019 (FRIDAY)
#include<stdio.h>
#include<stdlib.h>
#include<conio.h>
#include<iostream>
#include<time.h>
#include<chrono>
#include<thread>
#include<iomanip>
using namespace std;

//All definitions go here:
int lol;
int pc, quan, q2, subt;
char mem;
int option;

int price()
{
	printf("+--------------+---------------------+------------------+------------------+\n");
	printf("| Product Code | Product Description | Retail Price(RM) | Special Discount |\n");
	printf("+--------------+---------------------+------------------+------------------+\n");
	printf("|     101      |    Wall Scrapper    |      100.0       |        -         |\n");
	printf("|     202      |     Tiles Waxes     |      350.0       |        -         |\n");
	printf("|     303      |   Mud/Tar Remover   |      500.0       |   20%% Discount   |\n");
	printf("|     404      |      Dry Blower     |      850.0       |   25%% Discount   |\n");
	printf("+--------------+---------------------+------------------+------------------+\n");
	system("pause");
	return 0;
}

int main()
{
	printf("Initialising...\n");
	using namespace std::this_thread;
	using namespace std::chrono;
	sleep_for(seconds(2));
	sleep_until(system_clock::now() + seconds(1));
	printf("\nReady!\nBestPrice Mall Point of Sales Program\nversion 1.0\n");
	printf("Welcome!\n");
	printf("_#####___#####__\n_#____#__#____#_\n_#____#__#____#_\n_#####___#####__\n");
	printf("_#____#__#______\n_#____#__#______\n_#####___#______\n");
	printf("BEST PRICE MALL\n");
	printf("Do you have a membership? (Y/N)\n");
	cin >> mem;

	printf("Select Options:\n");
	printf("1) Product & Price Details\n2) Price Calculator\n3) Delivery Charge Calculator\n");
	printf("4) Total Pay Amount Calculator\n5) Exit\nOption: ");
	cin >> option;
	switch (option)
	{
	case 1:
		printf("Product Listing\n");
		price();
		break;
	case 2:
		printf("Price Calculator\n");
		break;
	case 3:
		printf("Delivery\n");
		break;
	case 4:
		printf("Total payment\n");
		break;
	case 5:
		printf("Exit\n");
		break;
	default:
		printf("Error\n");
	}
	printf("You selected option %d\n", option);

	return 0;
}

//By Group Rendang
//Chiew Kar Heng
//Matthew Kong
//Low Cheng An
//Steven Soh
//DO NOT COPY!!
