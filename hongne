/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package swe1;

import java.util.ArrayList;
import java.util.Scanner;

/**
 *
 * @author Xuan Hong
 */
public class SWE1 {
public static String repeat(String s) {
        String[] words = s.split("\\s");
        ArrayList<String> words2 = new ArrayList<>();
        String result = "";
        int k = 0;
        for (String w : words) {
            words2.add(w);
        }
        ArrayList<Integer> index = new ArrayList<>();
        for (int i = 0; i < words2.size(); i++) {
            for (int j = i + 1; j < words2.size(); j++) {
                if (words2.get(i).equals(words2.get(j))) { 
                    index.add(j);
                    words2.set(i,"REPEAT");
                }   
                else{
                    break;
                }
            } 
        }
        for (Integer integer : index) {
            words2.set(integer, "");
        }
        for (String string : words2) {
            if(!string.equals("")){
                result += string+" ";
            }
        }
        result=result.replace("\\s+","");
        return result;
    }

    public static void main(String[] args) {
        System.out.println("Case 1: i want go go to  the the zoo" );
        System.out.println("Expect output: i want REPEAT to REPEAT zoo");
        System.out.println("real output: "+repeat("i want go go to  the the zoo"));
        //------------------------------------------
        System.out.println("Case 2: i want go go to the the the zoo" );
        System.out.println("Expect output: i want REPEAT to REPEAT zoo");
        System.out.println("real output: "+repeat("i want go go to the the the zoo"));
        //-------------------------------------------
         System.out.println("Case 3:i i i want go go to the the the zoo" );
        System.out.println("Expect output: REPEAT want REPEAT to REPEAT zoo");
        System.out.println("real output: "+repeat("i i i want go go to the the the zoo"));
          //-------------------------------------------
         System.out.println("Case 4:i i want go go to go the the zoo zoo" );
        System.out.println("Expect output: REPEAT want REPEAT to go REPEAT REPEAT");
        System.out.println("real output: "+repeat("i i want go go to go the the zoo zoo"));
          //-------------------------------------------
         System.out.println("Case 5: i want Go go to The the The zoo" );
        System.out.println("Expect output: i want Go go to The the The zoo");
        System.out.println("real output: "+repeat("i want Go go to The the The zoo"));
          //-------------------------------------------
         System.out.println("Case 6:i i i want Go go go to  the the zoo" );
        System.out.println("Expect output: REPEAT want Go REPEAT to REPEAT zoo");
        System.out.println("real output: "+repeat("i i i want Go go go to  the the zoo"));
    }
    
    }

   
    

