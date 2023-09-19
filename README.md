# Write_a_lab_report_to_find_the_sum_of_each_digits_of_a_long_number.

/*Name: Rohul Amin Fahad 
Id:1017
Batch:62nd. 
Q: Write a lab report to find the sum of each digits of a long number. */

 #include <stdio.h>

int main() {
    long long number, temp, sum = 0;
    
    printf("Enter a long number: ");
    scanf("%lld", &number);
    
   
    if (number < 0) {
        printf("Please enter a non-negative number.\n");
        return 1;
    }
    
    temp = number;
    
    while (temp > 0) {
        int digit = temp % 10; 
        sum += digit;
        temp /= 10;
    }
    
    printf("The sum of digits in %lld is %lld\n", number, sum);
    
    return 0;
}
Input: 12345678987654321

Output:81

