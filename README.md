# Java
Some notes about Java

# Strings
  Objects of the Strings are immutable.Everytime you use any method is the **String** class,actually creates and returns a brand new **String** object containing the modification.The orginal String is left untouched.
  
  **String**类中每一个看起来会修改**String**值的方法，实际上会创建一个全新的**String**对象，以包含修改后的字符串内容。而最初的**String** 对象则丝毫未动。例子。
  ```Java
    public class Immutable{
      public static String upcase(String s){
        return s.toUppCase();
      }
      public static void main(String[] args){
        Stirng q="how";
        System.out.println(q);  // "how"
        String qq=upcase(q);
        System.out.println(qq); // "HOW"
        System.out.println(q);  // "how"
      }
    }
  ```
