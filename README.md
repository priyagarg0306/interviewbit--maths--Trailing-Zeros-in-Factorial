# interviewbit--maths--Trailing-Zeros-in-Factorial

**-----> Question:**

Given an integer A, return the number of trailing zeroes in A!.

Note: Your solution should be in logarithmic time complexity.



**Problem Constraints**
1 <= A <= 10000



**Input Format**
First and only argumment is integer A.



**Output Format**
Return an integer, the answer to the problem.



**Example Input**
Input 1:

 A = 4
Input 2:

 A = 5


**Example Output**
Output 1:

 0
Output 2:

 1


**Example Explanation**
Explanation 1:

 4! = 24
Explanation 2:

 5! = 120
 
 
 **-----> code:**
 
 int Solution::trailingZeroes(int A) {
int a=0,p=1,i=0;
while(A>=i){
    i=pow(5,p);
    a=a+A/i;
    p++;
}

return a;

}
