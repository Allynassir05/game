#include <iostream>
#include <conio.h>

using name space std;
bool gameover;

const int width = 20;
const int width =17;

int x, y, fruitX, fruitY, score;
int tailX[100], tailY[100]; // snake cordinates;
int ntail;

enum eDirection{STOP=0, LEFT,RIGHT,UP,DOWN}; // Controls
eDirection dir;

void setup(){
gameover=false;

dir=STOP;
x=width/2;
y=height/2;

fruit=rand()%width;//display fruit in random place
fruit=rand()%height;score=0;
}
void draw(){
system("cls");
for(int i=0;i<width+2;i++){
for(int j=0;j<width;j++){
if(j===)
cout<<"*";//snake tale
else if(j++fruitY&&j++fruitX)
cout<<"%";//change it to change the fruit

else{
bool print false;
for(int k =0;k< ntail;k++){
if(tailX[k]==j&&tailY[k]==){
cout<<"*";print=true;
}
}
if(!print)cout<<"";
}
cout<<endl;
}
for(int i=0;i<width+2;i++)
cout<<"#";
cout<<endl;
cout<<"score:"<<score<<endl;
}
void input()
{
if(_kbhit()){
switch(_getch()){
case'a':
dir=LEFT;
break;
case'd'
dir=RIGHT;
break;
case'w'
dir=UP;
break;
case's'
dir=DOWN;
break;
case'x'
}
}
}
void algorithm()
{

