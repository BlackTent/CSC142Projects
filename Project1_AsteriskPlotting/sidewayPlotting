public class SidePlot
{
    public static String PLOT_CHAR = "*";
    public static void main(String[] args){
        plotXSquared(-6,6);
        plotAbsXplus1(-5,5); 
        plotNegXSquaredPlus20(-4,4);
        plotSinWave(-9,9);
    }
    public static void plotXSquared(int minX, int maxX){ 
        System.out.println("Sideways Plot");
        System.out.println("y = x*x where " + minX + "<=x<=" + maxX);
        for(int row = maxX; row >= minX; row--){
           if (row != 0){
               System.out.print(" |");
               for(int col = 0; col < row * row; col++){
                   System.out.print(" ");
             }
           }
           if (row == 0){
               System.out.print("-*");
               for(int xAxis = 0; xAxis <= maxX * maxX; xAxis++){
                   System.out.print("-");
               }
           }
           else {
               System.out.print(PLOT_CHAR);
            } 
               System.out.println();
            }
    }
    public static void plotAbsXplus1(int minX, int maxX){
        System.out.println("Sideways Plot");
        System.out.println("y = |x| + 1, where " + minX + "<=x<=" + maxX);
        for(int row = maxX; row >= minX; row--){
            if (row != 0){
               System.out.print(" |");
               for(int col = 1; col < Math.abs(row) + 1; col++){
                    System.out.print(" ");   
               }
            }
            if (row == 0){
               System.out.print("-+*");
               for(int xAxis = 0; xAxis <= maxX; xAxis++){
                   System.out.print("-");
               }
            }
            else {
                System.out.print(PLOT_CHAR);
            }
            System.out.println();
        }
    }
    public static void plotNegXSquaredPlus20(int minX, int maxX){
        System.out.println("Sideways Plot");
        System.out.println("y = -(x*x)+20, where " + minX + "<=x<=" + maxX);
        for(int row = maxX; row >= minX; row--){
            if (row != 0){
                System.out.print(" |");
                for(int col = 0; col < -(row * row) + 20; col++){
                    System.out.print(" ");   
                }
            }
            if (row == 0){
                System.out.print("-+");
                for(int xAxis = 0; xAxis <= -(row * row) + 20 - 1; xAxis++){
                   System.out.print("-");
                }
                System.out.print(PLOT_CHAR);
            }    
            else {
                 System.out.print(PLOT_CHAR);
            }
            System.out.println();
        }
    }
    public static void plotSinWave(int minX, int maxX){
        System.out.println("Sideways Plot");
        System.out.println("y = 20sin(0.5x)+20, where " + minX + "<=x<=" + maxX);
        for(int row = maxX; row >= minX; row--){
            if (row != 0){
                System.out.print(" |");
                for(int col = 0; col < (20 * Math.sin(.5 * row))+20; col++){
                 System.out.print(" ");   
                }
            }
            if (row == 0){
                System.out.print("-+");
                for(int xAxis = 0; xAxis <= (20 * Math.sin(.5 * row))+20  ; xAxis++){
                   System.out.print("-");
                }
                System.out.print(PLOT_CHAR);
                for(int xAxis = 0; xAxis <= (20 * Math.sin(.5 * row))+20  ; xAxis++){
                   System.out.print("-");
                }
            }
            else {
                System.out.print(PLOT_CHAR);
            }
            System.out.println();
        }
    }
}

 
