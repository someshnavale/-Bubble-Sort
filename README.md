# -Bubble-Sort

An example implementation of BubbleSort in C++:
 void bubbleSort(vector<int>numbers)
 {
 for(int i = numbers.size() - 1; i >= 0; i--) {
 for(int j = 1; j <= i; j++) {
 if(numbers[j-1] > numbers[j]) {
 swap(numbers[j-1],numbers(j));
GoalKicker.com – Algorithms Notes for Professionals 145
 }
 }
 }
 }



#C Implementation
void bubble_sort(long list[], long n)
{
 long c, d, t;
 for (c = 0 ; c < ( n - 1 ); c++)
 {
 for (d = 0 ; d < n - c - 1; d++)
 {
 if (list[d] > list[d+1])
 {
 /* Swapping */
 t = list[d];
 list[d] = list[d+1];
 list[d+1] = t;
 }
 }
 }
}


#Bubble Sort with pointer
void pointer_bubble_sort(long * list, long n)
{
 long c, d, t;
 for (c = 0 ; c < ( n - 1 ); c++)
 {
 for (d = 0 ; d < n - c - 1; d++)
 {
 if ( * (list + d ) > *(list+d+1))
 {
 /* Swapping */
 t = * (list + d );
 * (list + d ) = * (list + d + 1 );
 * (list + d + 1) = t;
 }
 }
 }
}
