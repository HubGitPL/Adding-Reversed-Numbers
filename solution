#include <iostream>
#include <string>

using namespace std;
/*
Sample input:
3
24 1
4358 754
305 794

Sample output:
34
1998
1
*/

void reverseNumber(int* doZmiany) {
    int nowaLiczba = 0;
    while (*doZmiany) {
        nowaLiczba *= 10;
        nowaLiczba += (*doZmiany % 10);
        *doZmiany /= 10;
    }
    *doZmiany = nowaLiczba;
}
void solution(int* first, int* second) {
    int end = *first + *second;
    reverseNumber(&end);
    cout << end << '\n';
}
int main() {
    int a, b, c;
    cin >> a;
    for (int i = 0; i < a; i++) {
        cin >> b >> c;
        reverseNumber(&b);
        reverseNumber(&c);
        solution(&b, &c);
    }
}
