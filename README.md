#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include<time.h>
 int main () {
     srand(time(0));
    int random_number =(rand()%100)+1;
    int no_of_guesses=0;
    int guessed;
    //  printf("the random number is =%d",random_number);
    do{
        printf("\nguess a number =");
        scanf("%d",&guessed);
            if(guessed>random_number){
                printf("lower number please!\n");
            }  else if(guessed<random_number){
                printf("higher number please!");
            }
                    no_of_guesses++;
    }while(guessed!=random_number);
    printf("\nyou gussed a number in %d attempts",no_of_guesses);
    
    return 0;
}
    // first game
