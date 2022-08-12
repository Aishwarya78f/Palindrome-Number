# Palindrome-Number
This repository contains the C program to check whether a number is Palindrome or not.
#include <stdio.h>
#include <string.h>
 
void isPalindrome(char str[]) {
    int t = 0;
    int k = strlen(str) - 1;
 
    while (k > t) {
        if (str[t++] != str[k--]) {
            printf("%s is not a palindrome\n", str);
            return;
        }
    }
    printf("%s is a palindrome\n", str); }

 int main() {
    isPalindrome("pssp");
    isPalindrome("aauurrnmsee");
    isPalindrome("oppo");
    isPalindrome(“kitten”);
    return 0; }
