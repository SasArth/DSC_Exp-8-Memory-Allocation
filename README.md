# DSC_Exp-8
## Memory-Allocation

### Code:-
```
#include <stdio.h>
#include <stdlib.h>

int main()
{	
	printf("dynamic memory allocation using malloc():\n\n");
	
	char *ptr = (char*) malloc(2);
	*ptr = 'a';
	printf("%c %d\n", *ptr, ptr);
	
	ptr++;
	
	*ptr = 'b';
	printf("%c %d\n\n\n\n", *ptr, ptr);
	
	
	
	// calloc()
	
	printf("dynamic memory allocation using calloc():\n\n");
	
	int i, n;
	
	int *ptr2 = (int*) calloc(3, 4);
	
	for(i = 0; i < 3; i++)
	{
		printf("Enter a number: ");
		scanf("%d", &ptr2[i]);
	}
	
	printf("\nEntered array of numbers:\n");
	
	for(i = 0; i < 3; i++)
	{
		printf("%d %d\n", ptr2[i], &ptr2[i]);
	}
	
	return 0;
}

```

### Ouput:-
![image](https://user-images.githubusercontent.com/124967782/230789875-a07a3c89-75a2-4c75-a938-439074a0d8c0.png)
