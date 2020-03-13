package testmigong;

import java.util.Scanner;

public class migong {

	static int[][] mig;  
	static int n; 
	static int min;
	
	
	
	
	public static void main(String[] args) {
		
		Scanner scanner = new Scanner(System.in);
		n = scanner.nextInt();
		min = n*n;
		mig = new int[n][n];
		
		for (int i = 0; i < n; i++) {
			for (int j = 0; j < n; j++) {
				
				mig[i][j] = scanner.nextInt();     
				
				
			}
		}
			digui(1, 1, 0);ֵ
			if (min==n*n) {
				System.out.println("No solution");
				
			}else {
				System.out.println(min);
			}
		

	}
	
	public static void digui(int x, int y, int count) {
		if (x==n-2&&y==n-2) { 
			min = Math.min(count, min);  ֵ
		}else {
			mig[x][y] = 1;
			if (y<n-1 && mig[x][y+1]==0) {
				digui(x, y+1, count+1); 
			}
			
			if (x<n-1 && mig[x+1][y]==0) {
				digui(x+1, y, count+1); 
			}
			if (x>1 && mig[x-1][y]==0) {
				digui(x-1, y, count+1); //
			}
			
			mig[x][y]=0; //
		}
	}

}
