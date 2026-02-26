```c
#define PAGE 45
#define START "21/2/2026"
#define FINISH "22/3/2026"

int main()
{

    char *process[] =
    {
        "0 Finding tools we need"
        "1 Finding commands with options we need"
        "2 "

    }

    char *commands[] = 
    {
        """0 gcc filename.type:

                0 What = [Making a outputfile]

                1 gcc -g filename.type = [Extra debugging information]""",

        "1 objdump -D name.out = [Reqular disassembly all]",

        "2 objdump -M intel -D name.out = [intel deisassembly all]",

        """3 gdb -q ./name.out:

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

                    1 x/number?b = [Give us first number of register-name addresses in one-byte format]

                    2 x/number?h = [Give us first number of register-name addresses in half-word(2bit) format]

                    3 x/number?w = [First hlaf-word of registers hexadecimal address in full-word(4bit) format]
    
                6 quit"""

        "4 bc -ql = [Calculator]"

    };

    return 0;

}
```

