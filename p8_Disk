#include <stdio.h>
#include <conio.h>

void main()
{
  int queue[100], n, head, i, j, k, seek = 0, diff;
  float avg;
  
  printf("*** FCFS Disk Scheduling Algorithm ***");
  printf("Enter the Size Of Queue\t");
  scanf("%d", &n);
  printf("Enter the Queue\t");
  
  for(i=1 ; i<=n ; i++)
  {
    scanf("%d", &queue[i]);
  }
  
  printf("Enter the initial head position\t");
  scanf("%d", &head);
  queue[0] = head;
  printf("\n");
  
  for(j=0 ; j<=n-1 ; j++)
  {
    diff = abs(queue[j+1] - queue[j]);
    seek += diff;
    printf("Move from %d to %d with Seek %d\n", queue[j], queue[j+1], diff);
  }
  
  printf("\n Total Seek Time is %d\t", seek);
  avg = seek / (float)n;
  printf("\n Average Seek Time is %f\t", avg);
}
