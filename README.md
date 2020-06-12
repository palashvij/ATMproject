# ATMproject

#include<iostream>
#include<stdlib.h>
using namespace std;

int atm_mahine(int netbalance)
    {
	    for(int j=0;j<=15;j++)
		{
			double withdrawamount, depositaccount;
		    int chooseoption;
			cout<<"\n";
			if(j==0)
			{
				cout<<"\t\t *** Automated Machine ***"<< endl;
				cout<<"\nChoose a Transaction:\n\n"<<endl;
			}
						
			cout<<"     MAIN SCREEN   "<<endl;
			cout<<"[1] Inquire Balance "<<endl;
		    cout<<"[2] Withdraw "<<endl;
			cout<<"[3] Deposit "<<endl;
			cout<<"[4] Quit "<<endl;
			cout<<endl;
			cout<<"Enter option:";
			cin>>chooseoption;
			switch(chooseoption)
			{
		     	case 1:
				cout<<"\n[[[% BALANCE INQUIRY %]]]\n";
				cout<<"\n Your current balance is RS "<< netbalance<< endl;
				continue;
								
				case 2:
				cout<<"\n[[[% WITHDRAW %]]]\n";
				cout<<"Enter amount in Rupees: ";
				cin>>withdrawamount;
				netbalance = netbalance - withdrawamount;
				cout<<"You withdrew RS: "<< withdrawamount<< endl;
				cout<<"Your remaining balance is RS: "<< netbalance<< endl;
				continue;

				case 3:
				cout<<"\n[[[% DEPOSIT %]]]\n";
				cout<<"Enter amount in RS: ";
				cin>>depositaccount;
				netbalance = netbalance + depositaccount;
				cout<<"You deposited RS: "<< depositaccount<< endl;
				cout<<"Your new balance is RS: "<< netbalance<< endl;
				continue;

				case 4:
				cout<<"\n***[[[% EXIT MODE %]]]***\n";
				system("cls");
				break;

				default:
				cout<<"\n That is an invalid choose option Plz enter correct chooseoption: \n";
				continue;
			}
			break;
		}
	return 0;
	}

void printstar(char ch , int n)
{
    for(int i=1;i<=n;i++)
    {
	    cout<<ch;
    }
    cout<<"\n";
}

double netbalance;

int main()
{
	system("cls");
    int PasswordForAccount;
    int SecurityPinCode ;
    system("color B0");
    cout<<"\n\t\t    ========================================"<< endl <<endl;
    cout<<"\t\t            ||   WELCOME TO ATM   ||"<< endl<<endl;
    cout<<"\t\t    ========================================\n\n"<< endl;
    printstar('*',80);

    cout<<"      **************  PASSWORD FOR KARAN      IS 5555   **************\n";
    cout<<"      **************  PASSWORD FOR SANDEEP    IS 6666   ************** \n";
    cout<<"      **************  PASSWORD FOR MOHAN      IS 7777   ************** \n";
    cout<<"      **************  PASSWORD FOR IMRAN      IS 8888   ************** \n\n\n";
    printstar('&',80);
    for(int j=1;j<=13;j++)
	{
	    if(j>=2 && j<=13)
		{
			cout<<"\n\n\t WELCOME AGAIN  \n\t   MAIN PAGE \n";
		}
		cout<<"PLEASE ENTER THE SECURITY PINCODE\n";
		cin>>SecurityPinCode;
		system("cls");
		if(SecurityPinCode == 1111)
		{
			cout<<"\n WELCOME KARAN \n";
            for (int j=0;j<3;j++)
			{
				cout <<"Enter Password For Account"<<endl;
				cin>>PasswordForAccount;
				double initialbalance = 10000;
				netbalance=initialbalance;
				if (PasswordForAccount==5555)
				{
					atm_mahine(10000);
				}
				else if(j==1)
				{
					cout<<"\nCard is captured\n";
				}
				else
					cout<<"Pls try again!!!\n";
			}

		}	
		if(SecurityPinCode == 2222)
		{
			cout<<"\n WELCOME SANDEEP \n";
			for (int j=0;j<3;j++)
			{
				cout <<"Enter Password For Account"<<endl;
				cin>>PasswordForAccount;
				double initialbalance = 10000;
				netbalance=initialbalance;
				if (PasswordForAccount==5555)
				{
					atm_mahine(10000);
				}
				else if(j==1)
				{
					cout<<"\nCard is captured\n";
				}
				else
					cout<<"Pls try again!!!\n";
			}
			
		}
		else if(SecurityPinCode == 3333)
		{
			cout<<"\n Wellcome MOHAN \n";
			for (int j=0;j<3;j++)
			{
				cout <<"Enter Password For Account"<<endl;
				cin>>PasswordForAccount;
				double initialbalance = 10000;
				netbalance=initialbalance;
				if (PasswordForAccount==5555)
				{
					atm_mahine(10000);
				}
				else if(j==1)
				{
					cout<<"\nCard is captured\n";
				}
				else
					cout<<"Pls try again!!!\n";
			}
			
		}
		else if(SecurityPinCode == 4444)
		{
			cout<<"\n WELCOME IMRAN    \n";
			for (int j=0;j<3;j++)
			{
				cout <<"Enter Password For Account"<<endl;
				cin>>PasswordForAccount;
				double initialbalance = 10000;
				netbalance=initialbalance;
				if (PasswordForAccount==5555)
				{
					atm_mahine(10000);
				}
				else if(j==1)
				{
					cout<<"\nCard is captured\n";
				}
				else
					cout<<"Pls try again!!!\n";
			}
		}
	}
}
           
