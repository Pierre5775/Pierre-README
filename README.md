# Pierre-README
# CS50- Python Final Project
An easy-to-use program that facilitates user's task to determine **Loan**, **Compound interest** and **Capitalization**  .
It calculates a bond's value, interest rate, pay-off period, debt value paid on the bond and amount paid until today . 

***For Loan enter L , for Compound enter C , for Capitalization enter Cap***  
* V0 = Debt Value
* a  = Bond Value
* n  = Number of periods(annual ,monthly, others,...)
* i  = Annual percentage interest rate
* 
  ***LOAN***  
**Must have one missing parameter and neither V0 , a, n or i can be a negative number unless it is the missing parameter that we are looking to determine**
<sub> calculation is determined under the following defintion* **def loan_calc(V0,a,n,i)** using the function  **(Matrix,V0,a,n,i) = loan_calc(V0,a,n,i)**
<sub> In the table Matrix the first[] reads horizontally and the second [] next to it reads vertically.
 <sub> In first line of the table Matrix[2][0] we get D1 which is the first loan payment
 pas = 0.0025 is the distance between i2 and i1 that are the interest between two periods.
 <sub> D1 = a - V0 * i is the first payment due.  Matrix[2][0]
 <sub> We calculate the value of new bedt values vi1 and vi2 using mathematical equations , then we take the value in between them , and  we extract the 4th parameter to start building the table. 
 * Matrix[3][0] = a - D1 (First interest value) .**Only in the first line ,the interest paid is equal to the Total amount paid until today**
 * As we go on , the table shows the **Total amount paid until today** and **the remaining total amount**
 * We can add each year paid interest to determine the year-to-date total interest paid.
 * If we receive or if we eneter a negative value we get the message " Impossible Calculation , Please Verify Data"
 *  I entered a formula to adjust the rectification to zero in the last bond .

   ***COMPOUND INTEREST***
   <sub> By applying this formula we can determine the compound interest by entreing three parameters that **can not be negative** 
   def comp_int(C,n,i):
    A = C*((1+i)**n) 

  ***CAPITALIZATION***
  <sub> By providing the payment value per period, the number of periods and the interest rate , this program provides an accurate value of :
  _**Total interest given after n period of time**
  _**Cumulative amount after np periods**
  
    
   
 

 

