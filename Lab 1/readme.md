
## Variable Decleration
'''c
int N;
int p = 0, memory = 10;
'''c
## Array Decleration or Initialization
'''c
int array[10] = {1, 2, 3, 4, 5, 6, 7,8, 9, 10};

Array Elements Insertion (User Input)

'''c
/*for ( initialize ; condition; increment ) {

   scanf statement(s);

}*/

//Implement in Program

for(p = 0; p<memory; p++)
    {
        scanf("%d ",&array[p]);
    }
## Print The Array Elements

/*for ( initialize ; condition; increment ) {

   printf statement(s);
}*/

//Implement in Program
'''c

for(p = 0; p<memory; p++)

    {
        printf("%d ", array[p]);
    }
'''c
## Array Reversing

/*for ( initialize ; condition; Decrement ) {

   printf statement(s);

}*/

//Implement in Program

'''c

for(p = memory-1; p>=0; p--)

    {
        printf("%d ", array[p]);
    }
'''c

## Array Access

/*if (index_value > index_size)

##printf("Overflow"); //The index location is not available.*/

//Implement in Program

'''c

if(p>100)
        {
            printf("Overflow");

            break;
        }
'''c

## End of File

/*while(Conditions){

Statements;

}*/

//Implement in Program

'''c

while(scanf("%d",&array[p]) != EOF)
    {
        p++;
    }
'''c
    
    // or
'''c
    
while(scanf("%d",&array[p]) == 1)
    {
        p++;
    }
'''c
