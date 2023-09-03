# Matrix_addition
import java.util.Scanner;
public class matrix_add
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int [][] mat1=new int[3][3];
        int [][] mat2=new int[3][3];
        int [][] mat3=new int[3][3];
        int i,j;
        System.out.println("Matrix 1:");
        for(i=0;i<3;i++)
        {
            for(j=0;j<3;j++)
            {
                System.out.print("Enter "+i+j+": ");
                mat1[i][j]=sc.nextInt();
            }
        }
        System.out.println("\nMatrix 2:");
        for(i=0;i<3;i++)
        {
            for(j=0;j<3;j++)
            {
                System.out.print("Enter "+i+j+": ");
                mat2[i][j]=sc.nextInt();
            }
        }
        System.out.print("\n");
        System.out.println("Added Matrix:");
        for(i=0;i<3;i++)
        {
            for(j=0;j<3;j++)
            {
                mat3[i][j]=mat1[i][j]+mat2[i][j];
                System.out.print(mat3[i][j]+" ");
            }
            System.out.print("\n");
        }
    }   
}
