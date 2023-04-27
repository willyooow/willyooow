package library system;
import javax.swing.*;
import java.util.*;
public class library system {
    public static void main(String[]args){
        Scanner scan=new Scanner(System.in);
         String asn = null;
        System.out.println("\t\t\t\t\t\t*****************************"
                                +"\n\t\t\t\t\t\t*  Welcome to NU library system  *"
                                +"\n\t\t\t\t\t\t*****************************");
        
                System.out.print("Firstname: ");
                String fname=scan.nextLine();
                System.out.print("Lastname: ");
                String lname=scan.nextLine();
                                System.out.print("Address: ");
                String address=scan.nextLine();
                                System.out.print("Contact Number: ");
                int contractnum=scan.nextInt();
                
        Room NC=new Book(fname,lname,address,contractnum); 
        NC.getDetails();
        NC.setBookType();
       
        NC.setRoomInfo();
        NC.getDetails1();
        NC.getBook();
        NC.getDetailss();
          NC.getDetailsfinal();
            JOptionPane.showMessageDialog(null,"Hi, " + fname + lname + 
                                          "\n  The book you have chosen is  " + getRoomType()
                                        + "\n  The price of the book is " );
        JOptionPane.showInputDialog(null," are u sure u want to reserve the book?");  
         
       if(asn == "yes" && asn == "Yes"){
           JOptionPane.showMessageDialog(null,"Reservation Success" );
       }else if(asn == "no" && asn == "No"){
           JOptionPane.showMessageDialog(null,"Reservation cancelled");
           
       }else {
           JOptionPane.showMessageDialog(null,"Reservation failed! Please enter valid answer" + JOptionPane.WARNING_MESSAGE);
       }
               
    }

    private static String getBookype() {
        throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
    }
    
}
    }
    
}
