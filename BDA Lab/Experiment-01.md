## Implement the following Data structures in Java 
##### a) Linked Lists b) Stacks c) Queues d) Set e) Map 

###### a) Linked Lists:

```
import java.util.LinkedList;
import java.util.Scanner;

public class LinkedLestDemo {
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        LinkedList<Integer> lis=new LinkedList<Integer>();
        boolean bool=true;
        while(bool){
            System.out.println("1: adding");
            System.out.println("2: adding at the start");
            System.out.println("3:adding at the last");
            System.out.println("4:size");
            System.out.println("5:getting");
            System.out.println("6:removing");
            System.out.println("7:delete fully");
            System.out.println("8:Full list");
            System.out.println("9:Exit");
            System.out.println("Select the below options:");
            int choice=sc.nextInt();
            switch(choice){
                case 1:
                    int given=sc.nextInt();
                    lis.add(given);
                    break;
                case 2:
                    int first=sc.nextInt();
                    lis.addFirst(first);
                    break;
                case 3:
                    int last=sc.nextInt();
                    lis.addLast(last);
                    break;
                case 4:
                    int siz=lis.size();
                    System.out.println("The size is:"+siz);
                    break;
                case 5:
                    int a=sc.nextInt();
                    System.out.println("The element at the index is:"+lis.get(a));
                    break;
                case 6:
                    int rem=sc.nextInt();
                    System.out.println("the element removed is:"+lis.remove(rem));
                    break;
                case 7:
                    lis.clear();
                    System.out.println("After the deletion of the full list:"+lis);
                    break;
                case 8:
                    System.out.println("the list is the:"+lis);
                    break;
                case 9:
                    bool=false;
                    break;
                default:
                    System.out.println("Choose the correct option");
                    


            }


        }
        
    }
}
```



