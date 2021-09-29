    Вариант 1
    задание в homework/main.c
    запускается через visul studio
    учитывается "-"
```c
	if (decimal < 0)
	{
		decimal *= -1;
		printf("-");
	}
```
    учитывается переполнение
```c
	if (num > 11 && int_size == 32)
	{
		printf("A lot of signs");
		exit(-1);
	}
	if (num > 20 && int_size == 64)
	{
		printf("A lot of signs");
		exit(-1);
	}
```
    нули в начале двоичного числа не записываются
```c
int8_t zero_flag = 0; // delites all zeros at the beggining of the number
...
	if (binary[j] == 1)
		{
			zero_flag = 1;
		}
		if (zero_flag == 1)
		{
			printf("%d", binary[j]);
		}
```