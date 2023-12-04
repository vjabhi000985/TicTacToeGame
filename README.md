# TicTacToe Game in Java

## Overview
This Java-based TicTacToe game utilizes AWT and Swing libraries to provide an interactive graphical user interface. The project aims to deliver a seamless gaming experience with clear visuals and two-player functionality.

## Features
- *User-friendly GUI:* Developed with AWT and Swing components for an intuitive interface.
- *Two-player mode:* Enables interactive gameplay between two participants.
- *Visual representation:* Clear and visually appealing representation of the TicTacToe game board.

## Screenshots
1. *Game Start:*
   ![Screenshot (13)](https://github.com/vjabhi000985/TicTacToeGame/assets/46738718/c658d684-eced-427f-b6e6-0c88701d8cc4)

2. *In Progress:*
  ![Screenshot (14)](https://github.com/vjabhi000985/TicTacToeGame/assets/46738718/6ff89923-1692-49ad-8a67-6f0f9b4aec4f)

3. *Game Over:*
  ![Screenshot (15)](https://github.com/vjabhi000985/TicTacToeGame/assets/46738718/93b2b090-d0f8-4081-875e-988a6243319c)
![Screenshot (16)](https://github.com/vjabhi000985/TicTacToeGame/assets/46738718/edc23805-0868-4569-8cc1-ac47086fd032)

## How to Play
1. *Run the Application:*
   - Execute the `TicTacToe.java` file to start the game.
   
2. *Enter Player Names:*
   - Input the names of the players to personalize the gaming experience.
   
3. *Make Moves:*
   - Click on the grid to make a move during your turn.
   
4. *Enjoy the Game:*
   - Immerse yourself in the classic TicTacToe gameplay and aim for victory!
  
## Dependencies
   - Java Development Kit 8
   - Sublime Text 4

## Credits
Developed By Pandey Abhishek Nath Roy

## Code Snippet
```java
// Sample code snippet for making a move
public void actionPerformed(ActionEvent e){
       for(int i=0;i<9;i++){
               if(e.getSource()==buttons[i]){
                      if(player1_turn){
                             if(buttons[i].getText()==""){
                                     buttons[i].setForeground(new Color(255,0,0));
                                     buttons[i].setText("X");
                                     player1_turn=false;
                                     textField.setText("O-Turn");
                                     check();
                                }
                       }
                       else{
                              if(buttons[i].getText()==""){
                                       buttons[i].setForeground(new Color(0,0,255));
                                       buttons[i].setText("O");
                                       player1_turn=true;
                                       textField.setText("X-Turn");
                                       check();
                               }
                       }
		}
	}
}
