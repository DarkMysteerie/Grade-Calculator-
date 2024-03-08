# Grade-Calculator-
A simple C++ program on calculating GWA.

#include <iomanip>
#include <iostream>
using namespace std;

  int main ()
  {
  const int Attendance = 10,
              Quiz = 20,
              Exam = 30,
              PerformanceTask = 40;
              
   float AttendancePer,
              QuizPer,
              ExamPer,
              PerformanceTaskPer,
              Average;
              
cout <<"----------------------GRADE CALCULATOR---------------------"<<endl;
cout <<"\t Quiz = 20%" <<endl;
cout <<"\t Attendance = 10%" <<endl;
cout <<"\t Exam = 30%" <<endl;
cout <<"\t Performance Task = 40%" <<endl;
cout <<"\n";
cout <<"What is the total percentage of your Quiz from (0-20%)?"<<endl;
cin >> QuizPer;

cout <<"What is the total percentage of your Attendance from (0-10%)?" <<endl;
cin >> AttendancePer;

cout <<"What is the total percentage of your Examination from (0-30%)?" <<endl;
cin >> ExamPer;

cout <<"What is the total percentage of your Performance Task from (0-40%)?" <<endl;
cin>> PerformanceTaskPer;

Average = QuizPer + AttendancePer + ExamPer + PerformanceTaskPer;

cout<<"\n";

if (Average <= 100 && Average >=98){
    cout<<" A+. You passed." <<endl;
} else if (Average == 97 && Average >= 95){
    cout <<"A-. You passed." <<endl;
} else if (Average == 94 && Average >= 90){
    cout<<"A. You passed." <<endl;
} else if (Average == 89 && Average >= 85 ){
    cout <<"B. You passed." <<endl;
} else if (Average == 84 && Average >= 80){
    cout <<"C. You passed." <<endl;
} else if (Average == 79 && Average >= 75){
    cout <<"D. You passed." <<endl;
} else {
    cout <<"F. You failed." <<endl;
}


return 0;
}
