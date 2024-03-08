# Pierre-README
# CS50- Python Final Project
# Financial Navigator
An easy-to-use program that facilitates user's task to determine **Loan, Certificate of Depositst** and **Compound Interest** unknown inputs ***For Loan enter L , for Certificate of Deposit enter C , for Compoud Interest enter Comp*** 

***LOAN***  
**Must have one missing parameter and neither V0 , a, n or i can be a negative number unless it is the missing input calculation is determined under the following defintion def loan_calc(V0,a,n,i)** using the function  **(Matrix,V0,a,n,i) = loan_calc(V0,a,n,i)**
- V0 = Debt Value
- a  = Bond Value
- n  = Number of periods(annual ,monthly, others,...)
- i  = Annual percentage interest rate

In the  Matrix table the first[] reads horizontally and the second [] next to it reads vertically.
In first line of the table Matrix[2][0] we get D1 which is the first loan payment pas = 0.0025 is the distance between i2 and i1 that are the interest between two periods.
D1 = a - V0 * i is the first payment due.  Matrix[2][0]
We calculate the value of new bedt values vi1 and vi2 using mathematical equations , then we take the value in between them and  we extract the 4th parameter to start building the table. 
 - Matrix[3][0] = a - D1 (First interest value) .**Only in the first line ,the interest paid is equal to the Total amount paid until today**
 - The table shows the **Total amount paid until today** and **the remaining total amount**
 - We add each year paid interest to determine the year-to-date total interest paid.
 - If user enters a negative value the program delivers " Impossible Calculation , Please Verify Data"
 - I entered a formula to adjust the rectification to zero in the last bond.
 - If returned value is lower than loan value
   
***CERTIFICATE OF DEPOSITS***
Program will be prompted the initial capital, number of periods, interest rate per period i percent.
Program determines:
- Capital after n period
- Acquired interest values
  
***COMPOUND INTEREST***
 By providing the payment value per period, the number of periods and the interest rate, the program provides an accurate value of :
- Total interest given after n period of time
- Cumulative amount after n periods
def comp_int(C,n,i):
    A = C*((1+i)**n) 
**In Certificate of Deposits and Compound Interest No imputs could be negative values**
**We recommand not providing 4 inputs**

  
    
   
 

 

