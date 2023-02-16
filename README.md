//------------------------------------------------------------------------------------------------------------------------------------//
//------------------------------------------------------------------------------------------------------------------------------------//
//-----------------------------------------------Hotel Management System-------------------------------------------------------------//
//------------------------------------------------------------------------------------------------------------------------------------//
//------------------------------------------------------------------------------------------------------------------------------------//
#include<iostream>
using namespace std;
void details()
{

    cout<<"   ______________________________________________________________________________________\n";
    cout<<"  |                    The Hotel Person Detail Listed Below:                             |\n";
    cout<<"  |______________________________________________________________________________________|\n";
    cout<<"  | The Three Brother's Restro & Louge (Owner): Mr.Prashant Shrestha                     |\n";
    cout<<"  | The Three Brother's Restro & Louge (Mannager): Mr.Shree Krishna Ale                  |\n";
    cout<<"  | The Three Brother's Restro & Louge (Receptionist): Mr.Roshan Dura                    |\n";
    cout<<"  | The Three Brother's Restro & Louge (Staff): Mr.Hari Stha                             |\n";
    cout<<"  | The Three Brother's Restro & Louge (Staff): Mr.Raju PYRRR                            |\n";
    cout<<"  | The Three Brother's Restro & Louge (Staff): Mr.Hari Stha                             |\n";
    cout<<"  |______________________________________________________________________________________|\n";
    cout<<"\n";
  	int i,n=5 ;
    string name;
	{
		cout<<"                              *Note:: Only(Staff) 5 Member detail can be added\n";
		cout<<"      Enter The Number of Member You Wanna Add : "<<endl;
		cin>>n;
		cout<<"\n";
		system("cls");
		 if (n<5){
		 
		for(i=0;i<n;i++)
		{  
			cout<<"Add A Member detail :"<<endl;
			cin>>name;
	cout<<"   ______________________________________________________________________________________\n";
    cout<<"  |                    The Hotel Person Detail Listed Below:                             |\n";
    cout<<"  |______________________________________________________________________________________|\n";
    cout<<"  | The Three Brother's Restro & Louge (Owner): Mr.Prashant Shrestha                     |\n";
    cout<<"  | The Three Brother's Restro & Louge (Mannager): Mr.Shree Krishna Ale                  |\n";
    cout<<"  | The Three Brother's Restro & Louge (Receptionist): Mr.Roshan Dura                    |\n";
    cout<<"  | The Three Brother's Restro & Louge (Staff): Mr.Hari Stha                             |\n";
    cout<<"  | The Three Brother's Restro & Louge (Staff): Mr.Raju PYRRR                            |\n";
    cout<<"  | The Three Brother's Restro & Louge (Staff): Mr.Hari Stha                             |\n";
    cout<<"  |*New "<<"The Three Brother's Restro & Louge (Staff):"<<name<<"                              |\n";
    cout<<"  |______________________________________________________________________________________|\n";
    cout<<"\n";
	

}
			

}
		 else
		 {
		cout<<"You cannot Add more than 5 Member"<<endl;
		}
	}
	
    cout << "                              Press 0 To Return The Restro Menu" << endl;    // Menu Call
    int choice;
    cin >> choice;
    if (choice == 0) {
        return;

    }

}
void number()
{
    cout<<"   ______________________________________________________________________________________\n";
    cout<<"  |                    The Hotel Telephone Number Available list:                        |\n";
    cout<<"  |______________________________________________________________________________________|\n";
    cout<<"  |The Three Brother's Restro & Louge (Owner's No.): Not Available                       |\n";
    cout<<"  |The Three Brother's Restro & Louge (Mannager's No.): Mr.Shree Krishna Ale (9814575138)|\n";
    cout<<"  |The Three Brother's Restro & Louge (Receptionist): Mr.Roshan Dura (9844751286)        |\n";
    cout<<"  |The Three Brother's Restro & Louge (Staff): Mr.Hari Stha(9847561728)                  |\n";
    cout<<"  |The Three Brother's Restro & Louge (Staff): Mr.Raju PYRRR(9866147285)                 |\n";
    cout<<"  |The Three Brother's Restro & Louge (Staff): Mr.Hari Stha (9874512368)                 |\n";
    cout<<"  |Counter Telephone No. 065-55448                                                       |\n";
    cout<<"  |______________________________________________________________________________________|\n";
    cout<<"\n";
    cout << "                              Press 0 To Return The Restro Menu" << endl;
    int choice;
    cin >> choice;
    if (choice == 0) {
        return;
    }
}
void room()
{

    cout<<"   ______________________________________________________________________________________\n";
    cout<<"  |                           Total Number Of Rooms -(100)                               |\n";
    cout<<"  |______________________________________________________________________________________|\n";
    cout<<"  |                            Room Under (10000-20000)Rs                                |\n";
    cout<<"  |(Single Bed)   Luxury Room :: 15 Room's (All Facilities Available)  RS:10000          |\n";
    cout<<"  |(Double Bed)   Luxury Room :: 20 Room's (All Facilities Available)  Rs:20000          |\n";
    cout<<"  |                            Room Under (5000-9000)Rs                                  |\n";
    cout<<"  |(Double Bed)   High Class Rooms :: 20 Room's (   Good Facilities  ) Rs:7500           |\n";
    cout<<"  |(Single Bed) Middle Class Rooms :: 15 Room's (   Good Facilities  ) Rs:5000           |\n";
    cout<<"  |           Family Package Rooms :: 30 Room's (   Good Facilities  ) Rs:9000           |\n";
    cout<<"  |                                                                                      |\n";
    cout<<"  |For More Information Go To >Menu>choose no.opt '2'>Contact Restro Manager             |\n";
    cout<<"  |______________________________________________________________________________________|\n";
    cout<<"\n";
    {
        string name,gender,email;                                                                       // detail input
        double num,age;
        cout<<"                   To Book Room Please Fillup Some Requirements\n";
        cout<<"                 \n";
        cout<<"                 - Enter Your Full Name::";
        cin>>name;
        cout<<"                 - Enter Your Age ::";
        cin>>age;
        cout<<"                 - Enter Your Gender ::";
        cin>>gender;
        cout<<"                 - Enter Your Mail ::";
        cin>>email;
        cout<<"                 - Enter Your Contact.no::";
        cin>>num;
        {
            const int NUM_ITEMS = 5;
            const double PRICES[NUM_ITEMS] = {10000, 20000, 7500 , 5000,9000};
            const std::string ITEMS[NUM_ITEMS] = {"                    (Single Bed) Luxury Room", "                    (Double Bed) Luxury Room", "\n                         (Double Bed)High Class Rooms", "                    (Single Bed) Middle Class Rooms","                    Family Package Rooms"};
            {
                int order[NUM_ITEMS];
                int num_orders = 0;

                int choice;
                while (true) {
                    system("cls");
                    cout << "                                Please choose Room from the menu:" << endl;
                    for (int i = 0; i < NUM_ITEMS; i++) {
                        cout << i + 1 << ". " << ITEMS[i] << " - Rs" << PRICES[i] << endl;
                    }
                    cout<<"\n";
                    cout << "0. Finish Booking" << std::endl;
                    cout << "Please Enter A Room Located Number that You Needed > ";
                    cin >> choice;

                    if (choice == 0) {
                        break;
                    }
                    else if (choice < 1 || choice > NUM_ITEMS) {
                        std::cout << "Invalid selection, please try again." << std::endl;
                    }
                    else {
                        order[num_orders++] = choice - 1;
                    }
                }
                system("cls");
                double total = 0.0;
                cout << "                               Room Available:";
                cout<<"/n";
                {
                    system("cls");
                    cout<<"   ______________________________________________________________________________________\n";
                    cout<<"  |                           Identity Of The Guest                                      |\n";
                    cout<<"  |______________________________________________________________________________________|\n";
                    cout<<"  |                                                                                      \n";
                    cout<<"  |               Full Name:"<<name<<"                                                   \n";
                    cout<<"  |                  Age   :"<<age<<"                                                    \n";
                    cout<<"  |                Gender  :"<<gender<<"                                                 \n";
                    cout<<"  |                E-mail  :"<<email<<"                                                  \n";
                    cout<<"  |              Phone number:"<<num<<"                                                  \n";
                    cout<<"  |                                                                   threebrothersrestro\n";
                    cout<<"  |______________________________________________________________________________________|\n";
                    cout<<"\n";
                }
                for (int i = 0; i < num_orders; i++) {
                    int item = order[i];
                    cout << ITEMS[item] << " - Rs " << PRICES[item] <<endl;
                    total += PRICES[item];
                }
                cout << "\n                   Your Total Price: RS " << total <<endl;
                cout<<"\n";
                cout <<"\n                            Thankyou For  Trusting Our Service";
            }

        }

    };

    cout << "\n                              Press 0 To Return The Restro Menu" << endl;
    int choice;
    cin >> choice;
    if (choice == 0) {
        return;
    }
}
void enjoy()
{
    cout<<"   ______________________________________________________________________________________\n";
    cout<<"  |                               Fest Concert 2023                                      |\n";
    cout<<"  |______________________________________________________________________________________|\n";
    cout<<"  |                                                                                      |\n";
    cout<<"  |                                                                                      |\n";
    cout<<"  |                                                                                      |\n";
    cout<<"  |                               Available Soon!!!                                      |\n";
    cout<<"  |                                                                                      |\n";
    cout<<"  |                                                                                      |\n";
    cout<<"  |                                                                                      |\n";
    cout<<"  |______________________________________________________________________________________|\n";
    cout<<"\n";
    cout << "                              Press 0 To Return The Restro Menu" << endl;
    int choice;
    cin >> choice;
    if (choice == 0) {
        return;
    }
}
void items()

{
    const int NUM_ITEMS = 5;
    const double PRICES[NUM_ITEMS] = {5.99, 8.99, 7.99, 1.99,2.55};
    const string ITEMS[NUM_ITEMS] = {"Hamburger", "Pizza", "Salad", "Soft Drink","Burger"};
    {
        int order[NUM_ITEMS];
        int num_orders = 0;

        int choice;
        while (true) {
            system("cls");
            cout << "Please choose an item from the menu:" << endl;
            for (int i = 0; i < NUM_ITEMS; i++) {
                cout << i + 1 << ". " << ITEMS[i] << " - $" << PRICES[i] << endl;
            }
            cout << "0. Finish ordering" << std::endl;
            cout << "> ";
            cin >> choice;

            if (choice == 0) {
                break;
            }
            else if (choice < 1 || choice > NUM_ITEMS) {
                cout << "Invalid selection, please try again." << endl;
            }
            else {
                order[num_orders++] = choice - 1;
            }
        }
        system("cls");
        double total = 0.0;
        std::cout << "Your order:" << endl;
        for (int i = 0; i < num_orders; i++) {
            int item = order[i];
            cout << ITEMS[item] << " - $" << PRICES[item] << endl;
            total += PRICES[item];
        }
        cout << "Total: $" << total << endl;
    }
    int choice;
    cin >> choice;
    if (choice == 0) {
        return;
    }
}


void exit ()
{
    cout<<"  \n";
    cout<<"  \n";
    cout<<"  \n";
    cout<<"                                                                 ~~~~THANK YOU~~~~                                                              \n";
    cout<<"                                                  ~~~~~~~~~~~~FOR TRUSTING OUR SERVICE~~~~~~~~~~~~~~~                                                                 \n";
    cout<<"                    \n";
    cout<<"                    \n";
    cout<<"                    \n";
    cout<<"\n";
    cout<<"\n";
    cout<<"\n";
    cout<<"\n";
    cout<<"\n";
    cout<<"\n";
    cout<<"\n";
    cout<<"\n";
    cout<<"\n";
    cout<<"                                             A Short Project By   :  Prashant Rb_Shrestha\n";
    cout<<"\n";
    cout<<"                                                                         Roshan Dura\n";
    cout<<"\n";
    cout<<"                                                                     Shree Krishan Ale\n";
    cout<<"\n";
    cout << "                              " << endl;
    int choice;
    cin >> choice;
    if (choice == 0)
    {
        return;

    }
}
void drink()
{
    const int NUM_ITEMS = 5;
    const double PRICES[NUM_ITEMS] = {5.99, 8.99, 7.99, 1.99,2.55};
    const std::string ITEMS[NUM_ITEMS] = {"Soft Drink", "Khukuri Rum", "Black label", "Everest beer","Royal Treasure"};
    {
        int order[NUM_ITEMS];
        int num_orders = 0;

        int choice;
        while (true) {
            system("cls");
            cout << "                                    Please choose a drink from the menu:" << endl;
            for (int i = 0; i < NUM_ITEMS; i++) {
                cout << i + 1 << ". " << ITEMS[i] << " - $" << PRICES[i] << endl;
            }
            cout<<"\n";
            cout << "0. Finish ordering" << std::endl;
            cout << "> ";
            cin >> choice;

            if (choice == 0) {
                break;
            }
            else if (choice < 1 || choice > NUM_ITEMS) {
                std::cout << "Invalid selection, please try again." << std::endl;
            }
            else {
                order[num_orders++] = choice - 1;
            }
        }
        system("cls");
        double total = 0.0;
        std::cout << "Your order:" << std::endl;
        for (int i = 0; i < num_orders; i++) {
            int item = order[i];
            std::cout << ITEMS[item] << " - $" << PRICES[item] << std::endl;
            total += PRICES[item];
        }
        std::cout << "Total: $" << total << std::endl;
    }
    int choice;
    cin >> choice;
    if (choice == 0) {
        return;
    }
}

void fac()
{
    cout<<"   ______________________________________________________________________________________\n";
    cout<<"  |                              Facilities OF Restro                                    |\n";
    cout<<"  |______________________________________________________________________________________|\n";
    cout<<"  |        1. Swimming Pool (*4)                                                         |\n";
    cout<<"  |        2. Daily Live Concert                                                         |\n";
    cout<<"  |        3. Night Club                                                                 |\n";
    cout<<"  |        4. Every Floor With lift Facilities                                           |\n";
    cout<<"  |        5. Love Garden                                                                |\n";
    cout<<"  |        6. Fun Park                                                                   |\n";
    cout<<"  |                                                                                      |\n";
    cout<<"  |______________________________________________________________________________________|\n";
    cout<<"\n";
    cout << "                              Press 0 To Return The Restro Menu" << endl;
    int choice;
    cin >> choice;
    if (choice == 0) {
        return;
    }
}
int main()
{

    int a;

// 	string Username;
// 	string Password;
// 	cout<<"---------------------------------------------------------------------Welcome -------------------------------------------------------------------------------\n";
// 	cout<<"\t                                     --------------------------To------------------------                                                       \n";
// 	cout<<"\t___________________________________________The Login Page Of Three Brother Resto & Louge__________________________________________________                          \n";
// 	cout<<"\n";
// 	cout<<"\n";
// 	cout<<"\n";
// 	cout<<"----------------------------Enter The Requirements below | | | |\n";
// 	cout<<"\t                                                 v v v v\n";
// 	cout<<endl;
// do	{
// 	cout<<"                                     Enter Username::";
// 	cin>>Username;
// 	if(Username=="Admin") {
//        cout << "                               Enter Password::";
//        cin >> Password;
//        {
//            if (Password == "Admin") {
//                cout << "Thankyou For Login";
//            } else {
//                cout << "Please Enter the correct Password" << endl;
//            }
//        }
//    }
// 	else{
// 	    cout<<"Please Enter the correct username"<<endl;
// 	}
// }while(Username!="Admin" || Password!="Admin");

    {
        {
            while(true)
            { system("cls");
                cout<<"\t                                ____________Welcome_____________\n";
                cout<<" \t                                             TO                 \n";
                cout<<"\t                                   ---------The----------      \n";
                cout<<"\t                       -------------Three Brother's Restro & Louge-------------\n";
                cout<<"\t                                            Menu                  \n";
                cout<<"\t                                        Pokhar-2,Lakeside\n";
                cout<<"Contact no. Tel no.065-44587                                                            Mobile no. 9814182296\n";
                cout<<"                                                                           Gmail Threebrothersrstro24@gmail.com\n";
                cout<<"";
                cout<<"\n";
                cout<<"\n";
                cout<<"\n";
                cout<<"\t _____________________________________________________________________________________________________\n";
                cout<<"\t|                                          The Menu                                                   | \n";
                cout<<"\t|_____________________________________________________________________________________________________|\n";
                cout<<"\t|                           Enter(1)_To View: Hotel_Person Details                                    |\n";
                cout<<"\t|                           Enter(2)_To View: The Hotel Contact Number                                |\n";
                cout<<"\t|                           Enter(3)_To View: The Stylish Rooms                                       |\n";
                cout<<"\t|                           Enter(4)_To View: The Facilities Available in Hotel                       |\n";
                cout<<"\t|                           Enter(5)_To View: The Dishes Available                                    |\n";
                cout<<"\t|                           Enter(6)_To View: The Drinks                                              |\n";
                cout<<"\t|                           Enter(7)_To View: The Live Concert Date&Time Available In Hotel           |\n";
                cout<<"\t|                           Enter(8)_To View: To Exit                                                 |\n";
                cout<<"\t|_____________________________________________________________________________________________________|\n";
                cout<<"\n";
                cout<<"\t                           Select A Number(1-8)_That You Wanna A Visit::";
                int choice;
                cin>>choice;
                if(choice==1)
                {system("cls");
                    details();
                }
                else if(choice==2)
                {system("cls");
                    number();
                }
                else if(choice==3){
                    system("cls");
                    room();
                }
                else if(choice==4)
                {
                    system("cls");
                    fac();
                }
                else if(choice==5)
                {
                    system("cls");
                    items();
                }
                else if(choice==6){
                    system("cls");
                    drink();
                }
                else if(choice==7)
                {
                    system("cls");
                    enjoy();
                }
                else if(choice==8){
                    system("cls");
                    exit();
                }
                
                else{
                    cout<<"\n";
                    cout<<"                                  You Have entered wrong number :(\n                                   Please choose Number from 1-8";
                    break;
                }

            }
            return 0;
        }
    }
}





