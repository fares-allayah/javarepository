# javarepository

import java.util.Scanner;

public class JavaApplication19 {

    public static void main(String[] args) {
 
        Scanner scanner = new Scanner (System.in);
        System.out.print("Enter the number of rows:");
        int rows = scanner .nextInt();
    
        System.out.print("Enter the number of columns:");
    int columns = scanner .nextInt();
    
    int [][]array = new int [rows][columns];
    System.out.println("Enter the values of the array :");
    
    for(int i =0; i< rows;i++){
        for(int j =0; j< columns; j++){
            array[i][j] = scanner .nextInt();
        }
    }
    System.out.println("Original array:");
    printArray(array);
    int[][] reverseArray = reverseArray(array);
    System.out.println("Reverse array :");
    printArray(reverseArray);
    }
    public static void printArray(int [][] array ){
        for(int i = 0; i< array.length; i++){
            for(int j = 0; j < array[i].length; j++){
                System.out.print(array[i][j]  +" ");
            }
            System.out.println();
            }
        }
    
    public static int [][] reverseArray(int [][] array){
        int[][]reverseArray = new int[array.length][array[0].length];
        for (int i =0; i< array .length;i++){
            for (int j=0; j< array[i].length; j++){
                reverseArray[i][j] = array[array.length -1 - i][array[i].length - 1 - j];
            }
        }
        return reverseArray;
    }
        }
    
    
