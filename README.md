# 3-basamakli-armstrong-sayilarini-bulan-programm
#include <stdio.h>
#include <math.h>

int main () {

	
	
	int i;

	for ( i = 100; i <= 999; i++)
	{	
		int j = 0, value = 0, temp2 = i;
		
		while(j < 3)
		{	
		
			int temp = temp2 % 10;
			value = value + temp*temp*temp;
			temp2 = temp2 / 10;

			j ++;
		}

		if(value == i){
				printf(" %d ",value);
			}
	}
	
    
        return 0;
}
