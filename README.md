//CompoundAssignments
public class CompoundAssignment {
    public static void main(String[] args) {
        /* Advantages:short,easy to execute then usual. */
        int a=9,b=5;
        //a=a+b;
        a+=b;
        System.out.println(a);
    }
}
//Increment/DecrementOperator
public class IncrementDecrement {
    public static void main(String[] args) {
        byte a = 10;
        //Increment(or)Decrement Operator can be only used to add or minus only 1(one)value from its respective variable
        a++; //(Or) ++a; both are same
        --a;// (Or) a--; both are same
        System.out.println(a);
    }
}
//Relational Operator-Implementation using print module
public class RelationalOperations {
    public static void main(String[] args) {
        byte VariableOne = 10, VariableTwo =10;
        //System.out.println(VariableOne<100);
        System.out.println(VariableOne<=VariableTwo);
    }
}
/* Relational Operators majorly used in if conditions ( < > <= >= == !=)*/

/*BitwiseOperator
~NOT  
&AND  
|OR   
^EXOR  (very strict OR-true if one input as true and another input as false)
In Computer Memory Everything will be Stored in form of 0's and 1's(Transistor will be connected with the capacitor in the circuit)
if it get charged it is consider as 1, if not consider as 0 - as scale integration---1:36:48
in decimal number each will be consider as a digit, likewise binary number each will be consider as a bit
consider 5-101 bitwise operator will perform operation on each bit(handles it) but other operator perform operation by whole number
         6-110 at the background everything will be handled in bit wise manner don't see in that point of view view through programmer point of view

*/
In java negative numbers can be handled using 2s complement(which will be stored)
public class BitwiseOperator {
    public static void main(String[] args) {
             byte variableOne =9,variableTWo=12;
             int variableThree = variableOne & variableTWo;
             System.out.println(+variableThree);
             variableThree = variableOne | variableTWo;
             System.out.println(+variableThree);
             variableThree = variableOne ^ variableTWo;
             System.out.println(+variableThree);
             variableThree =  ~ variableTWo;
             System.out.println(+variableThree);


    }
}
Application of BitwiseOperators
.messages(encryption-decryption)--whatsapp
.networks parity checking,error codes
.Graphics-EXOR operator has been used

Swifting
<< Left Shift
>> Right Shift
>>> Right Swift Zero Fill
if we practice left shift(variableNmame << 1) then the lsb swift towards left 

/*
BooleanOperators
~NOT   <<  Left shift
&AND   >>  Right shift
|OR    >>> Right shift zeo fill
^EXOR
 */
 public class BooleanOperations{
            public static void main(string[] args){
                boolean a=true,b=false; //1-true 0-false we can also use compound assignment.
                System.out.println(a&b);
                System.out.println(a|b);
                System.out.println(a^b);
            }
}
/* Short circuit logical operators-it is special type of operator available in java(most of languages don't have this operator)
{
.&&(AND)-multiple
.||(OR) -Addition
} - check only first operand if it is flase,check both if first operand is true -02.00h
Boolean,Bitwise Operator check both operands
*/
 public class ShortCircuitLogicalOperation{
            public static void main(string[] args){
                int a=10;
                System.out.println((a>20) && (a<30)); //check whether the number is present between 20 to 30
                System.out.println((a<20) || (a>30)); // check whether the number is  not present between 20 to 30
            }
}//At some point of time,we may terminate to check another operand thats why this operator known as short circuit logical operator.
//Otherwise short circuit logical operator is used to combine relational 
 
