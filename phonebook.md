// combining the ideas of both numbers and string into one program

#include <stdio.h>
#include <strings.h>
int main(void)
{
    // Array of strings
    char *words[] = {"Nitish", "Sharma", "Pewcalypse"};
    char *numbers[] = {"+1-617-495-1000", "+1-617-495-1000", "+1-949-468-2750"};

    // ask user for string
    char name[50];
    printf("Name: ");
    scanf("%s", name);

    // search for name
    for (int i = 0; i < 3; i++)
    {
        if (strcasecmp(words[i], name) == 0)
        {
            printf("Found %s\n", numbers[i]);
            return 0;
        }
    }
    printf("Not found\n");
    return 1;
}
