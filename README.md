# PeakTraffic_Plate
//Program will notice to user if vehicle car go ahead in a determinated day and hour according las digit in the plate
// Monday 1 & 2 ; Tue 3 & 4 ; Wed 5 & 6 ; Thu 7 & 8 ; Fri 9 & 0
//hours do not allowed to go Morning 7 am thru 9:30 am  & Afternoon 16:00 trhu 19:30
class peakplate
{
public:
void plate();
void date();
void time();
};
void main()
{
int license_plate;
string date;
string hour;

void peakplate::plate()
{
int dig;
char day;
cout << "Enter License Plate Number" ;
cin >> license_plate;
dig = license_plate % 10;
if ( dig = 1 , 2){
   day = "Monday";
      if ( dig = 3 ,4){
      day = "Tuesday";
         if (dig = 5 , 6){  
         day ="Wednesday";
            if (dig = 7 , 8){
            day = "Thursday";
               if( dig = 9 , 0){
               day = "Friday";
               }
            }
         }
       }
   }
}  
void peakplate::date()
{
cout << "Enter date aaaa/mm/dd";
cin >> date;
function findaday(date); // call of a function that finds what day is the day in the date entered

}
void peakplate::time()
{
cout << "Enter 24 hour format hh:mm";
cin >> hour
//string mm(hour,3,2);
string hh(hour,0,2);
if day == date{
   if(7<hh<9 && 16<mm<19){
  cout << " do not go to traffic";
  }
  }
else
cout << " enjoy it!"
}
system("pause");
}
