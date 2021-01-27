# Missing-Element-in-the-Array
import java.util.*;
public class Main
{
	public static void main(String[] args) {
		//System.out.println("Hello World");
		Scanner scn = new Scanner(System.in);
		int[] arr = new int[10];
		int mis = 0, rep = 0;
		int[] c = new int[10];
		for(int i = 0; i < 10; i++){
		    arr[i] = scn.nextInt();
		    c[arr[i] -1]++;
		}
		for(int i = 0; i < 10; i++){
		    if(c[i] == 0){
		        mis = i+1;
		    }
		    if(c[i] > 1){
		        rep = i+1;
		    }
		}
		
		System.out.println(mis + " " + rep);
	}
}
