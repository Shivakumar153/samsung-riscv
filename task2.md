DEBUGGING USING SPIKE COMMAND
 
 riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c

![2](https://github.com/user-attachments/assets/fdd0fd8f-50a2-4819-b158-d887563a6653)

To start debugging we run the command

spike -d pk sum1ton.o 

![1](https://github.com/user-attachments/assets/c887d84f-0ed2-4303-97ac-50b717f5268c)


![3](https://github.com/user-attachments/assets/b4ca162b-5196-4891-aaa7-b15e90e32c3c)
