# To-find-whether-it-is-a-armstrong-number-or-not.










int main()
{
    int x = 3716;
    int y = x;
    int compare = y;
    int i,j,k,r;
    int n = 0;
    int sum = 0;
    int multiply;
    
    for (i=0; x>0;i++){
        x=x/10;
        n++;
    }
    
    for (k=0; y>0; k++) {
        multiply = 1;
        r=y%10; // find digit 
        y=y/10;
        for(j = 1; j <= n; j ++) {
        // multiply digit n times
            multiply = multiply*r;
        }
        sum = sum + multiply;
    }
    
    if(sum == compare) {
        printf("Armstrong number");
    } else {
        printf("Not an Armstrong number");
    }
