# SLEEP-TRACKER
1. Introduction
 A Sleep Tracker is a tool or application designed to monitor and analyze an individual’s sleep patterns over time. By tracking sleep duration and quality, users can identify habits affecting their sleep and improve their overall health and productivity. In this project, we aim to build a simple program to input daily sleep hours, calculate average sleep over a period, and provide feedback based on the data.

2. Ideation
To create a program that takes input of sleep hours for a week and analyze the average sleep duration of the user. 
Input daily sleep hours for 7 days. Calculate average sleep.m Provide feedback (e.g., “You are sleeping well,” “You need more rest,” etc.).

3. Analysis
Sleep hours of 7 days (can be float). 
Process: Sum the hours, calculate average, compare against recommended sleep duration 
Output: Average sleep hours and a message indicating sleep quality.

4. Built
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

5. Testing
The user should input the no. of hours a person slept during a week.

Output 1
Enter hours you slept on Day1: 8
Enter hours you slept on Day2: 9
Enter hours you slept on Day3: 7
Enter hours you slept on Day4: 8
Enter hours you slept on Day5: 9
Enter hours you slept on Day6: 9
Enter hours you slept on Day7: 8
Total hours you slept in the previous week is:58
Average hours you slept is:8.286You are sleeping well

Output 2
Enter hours you slept on Day1: 6
Enter hours you slept on Day2: 5
Enter hours you slept on Day3: 5
Enter hours you slept on Day4: 4
Enter hours you slept on Day5: 6
Enter hours you slept on Day6: 5
Enter hours you slept on Day7: 6
Total hours you slept in the previous week is:37
Average hours you slept is:5.286
You are not getting enough sleep. Try to rest more!!

6. Implementation
7. The project is published on google for easy access to the code.
8. https://github.com/Swaraj-web27/SLEEP-TRACKER

9. Conclusion
This simple sleep tracker program helps users understand their sleep patterns by collecting daily sleep hours and providing feedback on average sleep duration. Monitoring sleep is crucial for maintaining good health, and such programs encourage better habits.

