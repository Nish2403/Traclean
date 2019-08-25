#include<iostream.h>
#include<conio.h>
#include<stdio.h>
#include<fstream.h>
#include<string.h>

class traffic
{
private:

	char name[100];
	int age;

public:
char username[50];
char password[50];
void getdata()
{
	cout<<"Enter your name:";
	gets(name);
	cout<<"Enter your age:";
	cin>>age;
	cout<<"Enter your username:";
	gets(username);
	cout<<"Enter your password:";
	gets(password);
}
char getuser()
{
	return username[50];
}
char getpass()
{
	return password[50];
}
};

void main()
{
clrscr();
	char user[50],us[50],pa[50],pass[50];
	int i=0;
	traffic t;
	ifstream fin("tra.txt",ios::in);
	ofstream fout("tra.txt ",ios::out);
do{
	cout<<"                    TRAFFIC CLEAN             "<<endl;
	cout<<"                           -a application to clear traffic"<<endl;
	cout<<" ";
	cout<<" This app is a great work and very helpful to clear the todays traffic probles."<<endl;
	cout<<"This app is based on the principle where this app scans the location,"<<endl;
	cout<<"and scans for the cause for the traffic,and this app registers a complaint"<<endl;
	cout<<"traffic dept to take necessary actions with users permission only"<<endl;
	cout<<" "<<endl;
	cout<<" "<<endl;
	cout<<"1.login"<<endl;
	cout<<"2.Register"<<endl;
	cout<<"Enter any number:"<<endl;
	cin>>i;

if(i==1)
{
	clrscr();
	cout<<"USERNAME:"<<endl;
	gets(user);
	cout<<"PASSWORD:"<<endl;
	gets(pass);
	while(!fin.eof()){
	fin.read((char*)&t,sizeof(t));
	us[50]=t.getuser();
	pa[50]=t.getpass();
	}


if(strcmp(user,us)==0&&strcmp(pass,pa)==0)
{
clrscr();
	cout<<"login sucess"<<endl;
	cout<<"1.return to menu"<<endl;
	cout<<"3.exit"<<endl;
	cin>>i;
clrscr();
}
else
{
clrscr();
       cout<<"login failed"<<endl;
       cout<<"1.return to menu"<<endl;
       cout<<"3.exit"<<endl;
       cin>>i;
clrscr();
}}
if(i==2)
{
clrscr();
	t.getdata();
	fout.write((char*)&t,sizeof(t));
	clrscr();
	cout<<"registered sucessfully!"<<endl;
	cout<<"1.return to menu"<<endl;
	cout<<"2.exit"<<endl;
	cin>>i;
	clrscr();
}
fin.close();
fout.close();
}while(i==1);
	clrscr();
	cout<<"thank you!";


getch();
}





