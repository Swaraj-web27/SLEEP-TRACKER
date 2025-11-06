#include <stdio.h>
int main(){
    int day,sum=0;
    float average;
    for(int i=1;i<=7;i++){
        printf("Enter number of hours you slept on Day %d:",i);
        scanf("%d",&day);
        sum+=day;
    }
    average=sum/7.0;
    printf("\nAverage hours you slept is:%.3f",average);
    if(average>=9){
        printf("\nYou are sleeping too much. Consider consulting a health professional.");
    }
    else if(average>=8){
            printf("\nYou are sleeping well.");
    }
    else if(average>=7){
        printf("\nAverage sleep quality.");
    }
    else if(average>=6){
        printf("\nIncrease your sleeping time.");
    }
    else if(average<6){
        printf("\nYou are not getting enough sleep. Try to rest more!!!");
    }
    return 0;
}
