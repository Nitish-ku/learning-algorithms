// implement linear search for string

#include <stdio.h>
#include <string.h>

int main(void)
{
    // an array of string
    char *string[] = {"battleship", "boot", "cannon", "iron", "thimble", "top hat"};

    // ask user for string
    char s[50];
    printf("String: ");
    scanf("%s", s);

    // search for string
    for (int i = 0; i < 6; i++)
    {
        if (strcasecmp(string[i], s) == 0)
        {
            printf("found\n");
            return 0;
        }
    }
    printf("Not found\n");
    return 1;
}
