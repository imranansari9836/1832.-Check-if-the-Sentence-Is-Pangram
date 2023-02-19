class Solution {
    public boolean checkIfPangram(String sentence) {
       boolean[] A=new boolean[26];
       for(int i=0;i<sentence.length();i++)
       {
           A[sentence.charAt(i)-'a']=true;
       }
       for(boolean B:A)
       {
           if(!B)
           {
               return false;
           }
       } 
       return true;
    }
}
