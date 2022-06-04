/*Read an array of 'n' elements and find the second biggest number.
Your function should work for any type of data.
Sample I/O:
5
12 54 14 1 25
25
4
2.3 6.5 1.2 2.1
2.3*/

#include <iostream>
using namespace std;

template <typename T> 

T Sec_Big (T * A, int n)
{
    T max = -1, sec_max = -1;
    for (int i = 0; i < n; i++)
    {
        if (A[i] > max)
        {
            max = A[i];
        }
    }
    for (int i = 0; i < n; i++)
    {
        if (A[i] > sec_max && A[i] != max)
        {
            sec_max = A[i];
        }
    }
    return (sec_max);
}

int main ()
{
    int n;
    cin >> n;
    int * A = new int [n];
    float * B = new float [n];
    for (int i = 0; i < n; i++)
    {
        cin >> A[i];
    }
    int s1 = Sec_Big <int> (A, n);
    cout << s1 << endl;
    cin >> n;
    for (int i = 0; i < n; i++)
    {
        cin >> B[i];
    }
    float s2 = Sec_Big <float> (B, n);
    cout << s2 << endl;
}
