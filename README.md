# import java.util.*;
public class Door {

   private boolean open;

   public Door() {
     open=accessgranted;
   
   }
   public void Close(){
     open=accessdenied;
   }
  
   public void Open(){ 
     open=accessgranted;
   }  
     
}

public class LockDoor extends Door {

   protected boolean Lock;
   
   public LockDoor();
      Lock=accessdenied;   
   }

   public void Lock(){
      if(Open==accessdenied){
      Lock=accessgranted;
      }
      else {
         System.out.print("closing the door to lock it");
      
   }   
   
   public void UnLock(){
      if(Lock==accessgranted){
      Lock=accessdenied;
      }
      else { 
      System.out.print("unlocked already");
      
      }
   }
         
}
public class Program { 

   public static void main(String[] args) { 
   
     LockDoor d=new LockDoor();
     d.Lock();
     
     
   }// end of method

}// end of class
