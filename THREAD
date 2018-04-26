#include <stdio.h>
#include<stdlib.h>
#include<pthread.h>

int array[1000];


void * MyThread(void * arg);

int main()
{

	int i;

for(i=0;i<1000;i++)
{
	array[i]=i;
}

int sum=0;

	pthread_t t1;//,t2,t3,t4,t5,t6,t7,t8,t9,t10;

	pthread_create(&t1,NULL,MyThread,(void *)array[0]);
	//pthread_create(&t2,NULL,MyThread,(void *)array[100]);
	//pthread_create(&t3,NULL,MyThread,(void *)array[200]);
	//pthread_create(&t4,NULL,MyThread,(void *)array[300]);
	//pthread_create(&t5,NULL,MyThread,(void *)array[400]);
	//pthread_create(&t6,NULL,MyThread,(void *)array[500]);
	//pthread_create(&t7,NULL,MyThread,(void *)array[600]);
	//pthread_create(&t8,NULL,MyThread,(void *)array[700]);
	//pthread_create(&t9,NULL,MyThread,(void *)array[800]);
	//pthread_create(&t10,NULL,MyThread,(void *)array[900]);

	pthread_join(t1,sum);
	//pthread_join(t2,int Totalt2);
	//pthread_join(t3,int Totalt3);
	//pthread_join(t4,int Totalt4);
	//pthread_join(t5,int Totalt5);
	//pthread_join(t6,int Totalt6);
	//pthread_join(t7,int Totalt7);
	//pthread_join(t8,int Totalt8);
	//pthread_join(t9,int Totalt9);
	//pthread_join(t10,int Totalt10);

	//printf("%d",Totalt1+Totalt2+Totalt3+Totalt4+Totalt5+Totalt6+Totalt7+Totalt8+Totalt9+Totalt10)


	
return 0;

}

void * MyThread(void * arg)
{
	int i,sum=0;

int end;

end=(int)arg+100;

	for(i=(int)arg;i<=end;i++);
	{
		sum=sum+array[i];
	}
	pthread_exit(NULL);
}
