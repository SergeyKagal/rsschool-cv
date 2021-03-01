    1. Sergey Kagal
    2. Email 3461995@gmail.com 
    3. I'm a beginner front-end developer. I have no CS degree and have no experience in production. I am ready to work hard and learn programming.
    4. Experience in programming only in solving simple exercises from the books and Youtube.
    5. Example of my code:
```
#include <iostream>
const int SIZE=3;
using namespace std;// --don't do that, it's bad practice

struct Tquestion
{
    string question;
    string answer_option1;
    string answer_option2;
    string answer_option3;
    int correct_answer;
};

void List_init(Tquestion *qList)
{
  qList[0]={"what is the highest mountain in the world ?","Chomolungma","Dhaulagiri I","Nanga Parbat", 1};
  qList[1]={"who hasn't played a bond of these actors ?","Roger Moor","Martin Freeman","Timothy Dalton", 2};
  qList[2]={"What year did Depeche Mode release the album 'Violator'","1990","1985","1983", 1};
}
void ask(Tquestion *qList, int*p)
{
    int num;
    for(int i=0; i<SIZE; i++)
    {
        cout<<"\nQuestion #"<<i+1<<" \n"<<qList[i].question<<"\n\n";
        cout<<"1. "<<qList[i].answer_option1<<endl;
        cout<<"2. "<<qList[i].answer_option2<<endl;
        cout<<"3. "<<qList[i].answer_option3<<endl;
        cout<< "  Enter the number of correct answer: ";
        cin>>num;
            if(num==qList[i].correct_answer)
            {
                cout<<"Correct\n";
                (*p)+=100;
            }
            else cout<<"Incorrect\n";
    }
}
int main()
{
    Tquestion *qList=new Tquestion[SIZE];
    List_init(qList);
    int SCORE=0;
    int *pSCORE=&SCORE;
    ask(qList,pSCORE);
    cout<<"\n Your score :"<<SCORE;
    delete []qList;
    return 0;
}
```
    6.  
    7. BNTU graduate civil engineer.
    8. Various online English tests assess my level from beginner to intermediate. I translate texts using Google, I also perceive spoken language well.
