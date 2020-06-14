## Variable Decleration
```c
int i, j;
int X; // Where X is Value
int K; // Where K is Position or Index
int size = 10, tag = 0;
```
## Array Decleration or Initialization
```c
int array[100] = {1, 2, 3, 4, 5, 6, 7,8, 9, 10};
```
## Print The Array Elements
/*for ( initialize ; condition; increment ) {
   printf statement(s);
}*/

//Implement in Program
```c
for(i=0; i<size; i++)
        printf("%d ", a[i]);
```
## Insert Value in Array
//Insert Value
```c
scanf("%d", &X);
```
//Insert Position
```c
scanf("%d", &K);

for (i=size; i>=K; i--)
        a[i] = a[i - 1];
        
size++;

a[K - 1] = X;
```
## Update Index with Another Value
```c
for (i=0; i==K; i++)
        a[i] = a[i - 1];

a[K - 1] = X;
```
## Update Index with Another Value in a Correct Position or Index
//Insert Position
```c
scanf("%d", &K);
```
//Insert Value
```c
scanf("%d", &X);
for (i=0; i==K; i++)
      a[i] = a[i - 1];

a[K - 1] = X;
```
## Search a Value in Array
//Insert Value
```c
scanf("%d", &X);
for (i=0; i<size; i++){
      if(a[i]==X)
      tag++;
    }
```
## Search a Value in Array and if Found Print -1
```c
if(tag!=1)
   printf("-1");
```
## Delete a Value in Array
//Insert Position
```c
scanf("%d", &K);

for (i=K-1; i<size; i++)
       a[i] = a[i+1];
size--;
```
## Only Delete the First Occurrence of The Value
//Insert Value
```c
    scanf("%d",&X);

for(i=0; i<size; i++){
        if(X==array[i]){
            for(j=i; j<=size; j++){
                array[j] = array[j+1];
            }
            tag++;
            break;
        }
    }

size--;

if(tag!=1){
        printf("Not Found");
    }
    else{
        for(i=0; i<size; i++)
            printf("%d ",array[i]);
    }
```
## Delete All the Occurrence of The Value
//Insert Value
```c
scanf("%d",&X);

for( i=0; i<=size; i++){
        if(X==array[i]){
            for(j=i; j<=size; j++){
                array[j] = array[j+1];
            }
            size--;
            tag++;
            i--;
        }
    }
    
if(tag==0){
        printf("Not Found");
    }
    else{
        for(i=0; i<size; i++)
            printf("%d ",array[i]);
    }
```
