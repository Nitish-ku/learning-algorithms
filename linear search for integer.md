# learning-algorithms
learning about algorithms 

// implement linear search for integers

#include <stdio.h>
#include <string.h>

int main(void)
{
    // an array of integers
    int numbers[] = {20, 500, 10, 5, 100, 1, 50};

    // ask user for number
    int n;
    printf("Number: ");
    scanf("%i", &n);

    // search for number
    for (int i = 0; i < 7; i++)
    {
        if (numbers[i] == n)
        {
            printf("Found\n");
            return 0;
        }
    }
    printf("Not found\n");
    return 1;
}
