```c
#define PAGE 45
#define START "21/2/2026"
#define FINISH "22/3/2026"

int main()
{
    char *commands[] = 
    {
        """gcc filename.type:

                0 What = [Making a outputfile]

                1 gcc -g filename.type = [Extra debugging information]""",

        "objdump -D name.out = [Reqular disassembly all]",

        "objdump -M intel -D name.out = [intel deisassembly all]",

        """gdb -q ./name.out:

            0 What = [Debugging]

            1 Commands:

                0 break function-name = [Chosing breaking point for run in a functions]

                1 run = [Run program]

                2 info x:

                    0 registers

                3 list = [Cat do]

                4 disassemble function-name = []

                5 (x/o hexadecimal-address = [Octal], x/x $register-name [Hexadecimal], x/u $register-name = [Base 10 decimal], x/t $register-name = [Binary]):
 
                    0 x/number? $register-name = [Give us first number of register-name addresses] 

                    1 x/number?b = [Give us first number of register-name addresses in two-byte format]

                    2 x/number?h = [Give us first number of register-name addresses in half-word format]

                    3 x/number?w = [First hlaf-word of registers hexadecimal address in full-word format]
    
                6 quit"""

    };

    return 0;

}
```

