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
int prevX=tailX[0];
int prevY=tailY[0];
int prev2X,prev2Y;
tail[0]=x;
tail[0]=y;
for(int i=1;i<ntail;i++){
prev2X=tailX[i];
prev2Y=tailY[i];
tailX[i]=prevX;
tailY[i]=prevY;
prevX=prev2X;
prevY=prev2Y;
}
switch(dir){
case LEFT:
X--;
break;
case RIGHT:
X++;
break;
case DOWN:
y++;
break;
default:
break;
}
if (x>=width)x=0;else if(x<0)x=height-1;
if (y>=width)y=0;else if(y<0)y=height-1;
for (int i=0;i<ntail;i++)
if(tailX[i]==x&&tailY[i]==y)gameover=true;
if(x==fruitX&&Y==fruitY){score+=10;
fruitX=rand()%width;
fruitY=rand()%height;
nTail==;
}
}
int main()
{
setup();
while(!gameover){
Draw ();
input();
algorithm();
}
return 0;}
