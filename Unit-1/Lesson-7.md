## Lesson 7 Find a max prime number within 100 ��100���ڵ��������
	#include <stdio.h>
	#include <math.h>

	int main(void)
	{
		int sum;
		int i, j;
		int max = 0;
		int tmp;

		for (i = 1; i <= 100; i++)
		{
			tmp = (int)sqrt(i);

			for (j = 2; j <= tmp; j++)
			{
				if (i % j == 0)
					break;
			}

			if (j == tmp + 1)
				max = i;
		}

		printf("max = %d\n", max);

		return 0;
	}

* �﷨֪ʶ��
	- ��ѧͷ�ļ� math.h
	- ��ѧ�⺯�� sqrt
	- ǿ������ת�� (int)
	- �����߼�Ƕ��