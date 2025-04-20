#include <stdio.h>
#include <string.h>

typedef struct
{
    const char *name;
    char *number;
} person;

int main(void)
{
    person people[3];

    people[0].name = "Nitish";
    people[0].number = "+1-617-495-1000";

    people[1].name = "Sharma";
    people[1].number = "+1-617-495-1000";

    people[2].name = "Pewcalypse";
    people[2].number = "+1-949-468-2750";

    // user's input
    char num[50];
    printf("Name: ");
    scanf("%s", num);

    // search for name
    for (int i = 0; i < 3; i++)
    {
        if (strcasecmp(people[i].name, num) == 0)
        {
            printf("Found %s\n", people[i].number);
            return 0;
        }
    }
    printf("Not found\n");
    return 1;
}
