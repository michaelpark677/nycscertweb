# nycscertweb
New repo for my stuff.

This is for my stuff....


//contributors: David Moste, Jihae Park, Richard Parker, Moo Joon Park
//PROVIDE: provide both normal imports
import java.io.*;
import java.util.*;

//PROVIDE - wrapper for class
public class livecode{
  public static int findMaxValue( int[] data ) {
    //STUDENT-PROMPT: How should we start the method? What is the first thing we need?
    //STUDENT-PROMPT: What value should "m" be assigned at the start of the method?
    //MUST-ANSWER-Q: Why do we need variable "m"?
    //POSSIBLE FIRST DRAFT:
    int m = 0;

    //POSSIBLE REVISION:
    int m = data[0];

    //POSSIBLE DELIBERATE-ERROR: teacher types "int i = 0"
    //STUDENT-PROMPT: What is the exit condition of our array?
    for(int i = 1; i < data.length; i++){
      //STUDENT-PROMPT: How can we compare each item to the current max value and update?
      if(data[i] > m){
        m = data[i];
      }
    }
    //STUDENT-PROMPT: How do we get back the max value?
    return m;
  }

  //PROVIDE: main method to test the code
  public static void main(String[] args){
    int[] data = new int[]{3, 6, 9, 10, 2, 4, 22};

    int maxVal = findMaxValue(data);
  }
}
