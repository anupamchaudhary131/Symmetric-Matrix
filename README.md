# Symmetric-Matrix

public class DSA_Symmetric_matrix {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the no. of rows :");
        int m = sc.nextInt();
        System.out.println("Enter the no. of columns :");
        int n = sc.nextInt();
        int arr[][] = new int[m][n];
        System.out.println("Enter the elements in the matrix :");
        for (int i = 0; i < m; i++) {
            for (int j = 0; j < n; j++) {
                System.out.println("Enter the " + (i) + (j) + " element");
                arr[i][j] = sc.nextInt();
            }
        }

        System.out.println("The given matrix is :");
        for (int i = 0; i < m; i++) {
            for (int j = 0; j < n; j++) {
                System.out.print(arr[i][j]+" ");
            }
            System.out.println();
        }
        System.out.println("The Symmetric matrix is :");
        for (int i = 0; i < m; i++) {
            for (int j = 0; j < n; j++) {
                if(i==j)
                {
                    System.out.print(arr[i][j] +" ");
                }
                else
                {
                    System.out.print(arr[j][i] +" ");
                }
            }
            System.out.println();
        }
