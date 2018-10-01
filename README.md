# loginSystem
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package loginsystem;

import javax.swing.*;

/**
 *
 * @author linda
 */
public class LoginSystem {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        //creating a jframe
        JFrame myframe=new JFrame("Login ");
       myframe.setSize(400, 300); //size of the jframe
       myframe.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);// ensures the jframe is exited when closed
       myframe.setVisible(true);// ensure the jfarme is seen
       //creating a panel
       JPanel panel1=new JPanel();// creating the panel
       //creating buttons
       JButton loginbutton = new JButton();//creating a button
       loginbutton.setText("Log in");//gives the button a name
       loginbutton.setSize(100, 100); //gives the size of the button
       //displaying text using labels on the jframe
       JLabel namelabel=new JLabel("Username:");
       JLabel usernamelabel=new JLabel("Password:");
       JTextField Username=new JTextField();
       JTextField Password=new JTextField();
       Username.setColumns(10);
       Password.setColumns(10);
       //adding the details to the panel
       panel1.add(namelabel);
       panel1.add(Username);
       panel1.add(usernamelabel);
       panel1.add(Password);
       panel1.add(loginbutton);
       myframe.add(panel1);
    }
    
}
