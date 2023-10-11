import java.awt.Color;
import java.awt.Graphics;

public class GraphicsProject
{
    // Constants for the drawing size
    public static final int WIDTH = 400;
    public static final int HEIGHT = 400;
    public static final int WIDTH_2 = 600;
    public static final int HEIGHT_2 = 600;
    private static final int DOTS_PER_AXIS = 20;
    
    public static void main(String[] args){
        // Call Part 1
        drawCurvedLines();
       
        // Call Part 2
        drawShapes();
        
    }
    
    // Part 1: Generate curved lines
    public static void drawCurvedLines(){
        // Create the DrawingPanel
        DrawingPanel dp = new DrawingPanel (WIDTH,HEIGHT);
        Color bgColor = new Color(0,0,0);
        dp.setBackground(bgColor);
    
        Graphics g = dp.getGraphics(); 
        //a center to connect with otehr lines
        int centerX = WIDTH / 2;
        int centerY = HEIGHT / 2;
        
        for (int i = 0; i <= DOTS_PER_AXIS; i++){
            // Yellow lines
            g.setColor(new Color(255, 255, 0)); 
            
            // Draw right down side face East side diagonal line
            g.drawLine(WIDTH - ( i * 10), HEIGHT / 2, centerX + ( i * 7) ,centerY + ( i * 7));
            // Draw right down side face South diagonal line
            g.drawLine(WIDTH / 2, HEIGHT - ( i * 10), centerX + ( i * 7) ,centerY + ( i * 7) );
            
            // Draw left up side face West diagonal line
            g.drawLine(0 + ( i * 10),HEIGHT / 2,centerX - ( i * 7) , centerY - ( i * 7)); 
            // Draw up left  side face North diagonal line
            g.drawLine(WIDTH / 2, 0 + (i * 10),centerX - ( i * 7) , centerY- ( i * 7));
            
            // Draw right up side face East diagonal line
            g.drawLine(WIDTH - ( i * 10), HEIGHT / 2,centerX + (i * 7), HEIGHT / 2 - ( i * 7));
            // Draw up right  side face North diagonal line
            g.drawLine(WIDTH / 2, 0 + (i * 10) , centerX + (i * 7), centerY - ( i * 7));
            
            // Draw down left  side face West diagonal line
            g.drawLine(0 + ( i * 10), HEIGHT / 2,centerX - ( i * 7) , centerY + ( i * 7));
            // Draw down left  side face South diagonal line
            g.drawLine(WIDTH / 2,HEIGHT - ( i * 10), centerX - ( i * 7),centerY + ( i * 7));
        }
    }
        
    //Part 2: Create and draw filled shapes
    public static void drawShapes(){
        DrawingPanel dp = new DrawingPanel(WIDTH_2, HEIGHT_2);
        dp.setBackground(new Color(51,204,255));
        Graphics g = dp.getGraphics();
        
        drawFish1(g);
        drawFish2(g);
        drawRocks(g);
        drawWave(g);
        drawBoat(g);
    }
    
    //Function for draw fish in left sid
    public static void drawFish1(Graphics g){
        int x = WIDTH_2 / 3;
        int y = HEIGHT_2 / 3;
        for(int  i= 0; i < 20; i++){
            //Big Fish head
            g.setColor(new Color(255, 0, 0));
            g.fillRect(x + (i * 5), y - (i * 4), 4 , i * 8);
            //BigFish body
            g.setColor(new Color(255, 255, 0));
            g.fillRect(x + (i * 5) + 50, y - (i * 2), 4 , i * 4);
            //Big Fish eyes
            g.setColor(new Color(0, 0, 0));
            g.fillOval(x + 20, y-8 , 20, 20);
            //bubble
            g.setColor(new Color(0, 0, 255));
            g.drawOval(x - 20, y - 8, 20, 20);
            g.drawOval(x - 10, y - 30,15, 15);
            g.drawOval(x + 2,  y - 50, 0, 10);
        }
    }
    
    //Functon for fish in the right side
    public static void drawFish2(Graphics g){
        int x = WIDTH_2 / 6;
        int y = HEIGHT_2 / 2;
        for(int  i = 0; i < 15; i++){
            //Big Fish head
            g.setColor(new Color(102, 0, 153));
            g.fillOval(x + (i * 5) + 50,y - (i * 2), 4, i * 4);
            //BigFish body
            g.setColor(new Color(255, 204, 51));
            g.fillOval(x + (i * 5) + 80,y - i ,4, i * 2);
            //Big Fish eyes
            g.setColor(new Color(255, 102, 0));
            g.fillOval(x + 75, y - 7 , 10, 10);
            //bubble
            g.setColor(new Color(255, 255, 255));
            g.drawOval(x + 35, y - 8 , 15, 15);
            g.drawOval(x + 40, y - 30 , 12, 12);
            g.drawOval(x + 50, y - 50 , 10, 10);
        }
    }
       
    //Functon for fish in the right side
    public static void drawRocks(Graphics g){
        int x = WIDTH_2/2;
        int y = HEIGHT_2/2 ;
        for(int  i= 0; i < 15; i+=3){
            //Big rocks
            g.setColor(new Color(102,51,0));
            g.fillOval(x + (i*40),y +255,120, 100);
       
            //Small rocks
            g.setColor(new Color(153, 102, 0));
            g.fillOval(x - (i*40),y +247,80, 100);
        }
    }
    
     public static void drawWave(Graphics g){
        int x = WIDTH_2/2;
        int y = HEIGHT_2/9;
        for(int  i= 0; i < 20; i+=3){
            //Big rocks
            g.setColor(new Color(255,255,255));
            g.fillOval(x + (i*40),y -150,180, 200);
            g.fillOval(x - (i*40),y -150,180, 200);
        }
    }
    public static void drawBoat(Graphics g){
        int x = WIDTH_2/2;
        int y = HEIGHT_2/2;
        g.setColor(new Color(102,102,102));
        g.fillRect(x + 55 ,y - 225,100, 30);
        g.fillRect(x + 100 ,y - 290,5, 70);
        for(int  i= 0; i < 12; i++){
            g.setColor(new Color(255,0,0));
            g.fillRect(x + 55 ,y - 290,50, 30);
            g.setColor(new Color(255,255,255));
            //white strips
            g.fillRect(x + 55 ,y - 285,100, 1);
            g.fillRect(x + 55 ,y - 280,100, 1);
            g.fillRect(x + 55 ,y - 275,100, 1);
            g.fillRect(x + 55 ,y - 270,100, 1);
            g.fillRect(x + 55 ,y - 265,100, 1);
            g.fillRect(x + 55 ,y - 260,100, 1);
            // Blue rect
            g.setColor(new Color(0,0,255));
            g.fillRect(x + 55 ,y - 290,20, 15);
            g.drawString("America", x + 80, y - 205);
        }
    }
    
}  
