#include<unistd.h>
#include<stdio.h>
#include<fcntl.h>
#include<dirent.h>
#include<sys/types.h>
#include<sys/stat.h>

int main()

{

	pid_t a;

	int b,i;

	A:

	{

		printf("\n\nenter a positive integer number :");

		scanf("%d",&n);

		if(b>0)

		{

			printf("\n\nvalue is a positive integer. entered number is valid");

		}

		else

		{

			printf("\n\nentered number is not a valid positive integer. try another number");

			goto A;

		}

	}

	a=fork();

	if(a>0)

	{

		printf("\n\nParent process is being executed.....");

		sleep(10);

		printf("\n\nParent process execution is completed");

	}

	else

	{

		printf("\n\nChild process started execution");

		printf("\nSequence is ");

		printf("\n\t%d",b);

		for(i=0;i<b;i++)

		{

			if(b==2)

			{

				break;

			}

			else

			{

				b=b/2;

				printf("\t%d",,b);

			}

		}

		printf("\t1");

		printf("\n\nChild process execution completed");

	}
}
