#include <stdio.h>

int euclid(int a, int b)
{

    //1. If(b = 0) return a  // 종료조건 of 재귀호출!
    if (b == 0) return a;
    
    //2. return Euclid(b, a mod b)
    return euclid(b, a % b);

}

int test1_euclid()
{
    int gcd = 0;

    gcd = euclid(34, 48);
    printf("Hello World! %d\n", gcd);

    return 0;
}

int main(int argc, char * argv[])
{
    test1_euclid();
}
