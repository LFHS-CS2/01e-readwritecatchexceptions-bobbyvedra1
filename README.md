[![Work in Repl.it](https://classroom.github.com/assets/work-in-replit-14baed9a392b3a25080506f3b7b6d57f295ec2978f6f33ec97e36a161684cbe9.svg)](https://classroom.github.com/online_ide?assignment_repo_id=3049730&assignment_repo_type=AssignmentRepo)
Write code to copy each line from test.in into a new file called test.out.  Use the Internet to figure out how to do it.

When you are able to the "run tests" successfully, see if you can program it in a different way.

import java.io.*;
import java.util.*;
class Main {
    public static void main(String[] args)  {
      try
{
       Scanner in = new Scanner(new File("test.in"));
       PrintWriter out = new PrintWriter("test.out");
       while (in.hasNextLine()) {      
           out.println(in.nextLine());   
       }  
        in.close();   
        out.close();
}
catch (Exception e)
{
     System.out.println("exception");

}       
    }
}
