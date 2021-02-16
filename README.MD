<h1>Bubble Sort implementation in assembly.</h1>
<br/>
To implement the algorithm the Hack assembly language was used. Implementation was done according the pseudocode below.

<h2>Bubble Sort Algorithm in Pseudocode:</h2>
<br/>

```pseudocode
A[0]=5
A[1]=4
A[2]=3
A[3]=2
A[4]=1
A[5]=0

int j;
flag = 1;                          // set flag to true to begin first pass
int temp;                          // holding variable

while ( flag  == 1)
 {
    flag= false;                   // set flag to false awaiting a possible swap
    for( j=0;  j < 5;  j++ )
    {
         if (A[ j ] > A[j+1] )     // test for ascending sort
         {
             temp = A[ j ];        // swap elements
             A[ j ] = A[ j+1 ];
             A[ j+1 ] = temp;
             flag = 1;             // shows a swap occurred
          }
    }
}
```

Execution demonstration on CPU Emulator:

[![Bubble Sort in Hack Assembly language.](resource/BubbleSort.gif)](https://youtu.be/9C4eNMDfwbQ)


