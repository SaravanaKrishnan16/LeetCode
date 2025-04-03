Given n pairs of parentheses, write a function to generate all combinations of well-formed parentheses.

Example 1:

Input: n = 3
Output: ["((()))","(()())","(())()","()(())","()()()"]

Example 2:

Input: n = 1
Output: ["()"]
 
Constraints:

1 <= n <= 8

----------------------------------------------------------------------------------------------------------------

class Solution {
    public List<String> generateParenthesis(int n) {
        int oc=0,co=0;
        ArrayList<String> str = new ArrayList<>();
        String s = "";
        fun(oc,co,n,str,s);
        return str;
    }
    public static void fun(int oc,int co,int n,ArrayList<String> str,String s){
          if (s.length()==n*2) {
            str.add(s);
        }
        if(oc<n){
            fun(oc+1,co,n,str,s+"(");
        }
        if(co<oc){
            fun(oc,co+1,n,str,s+")");
        }
    }
}
