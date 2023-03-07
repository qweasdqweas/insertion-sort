# insertion-sort

삽입정렬
은 자료 배열의 모든 요소를 앞에서부터 차례대로 이미 정렬된 배열 부분과 비교하여, 자신의 위치를 찾아 삽입함으로써 정렬을 완성하는 알고리즘이다.

package project;

import java.util.Arrays;

public class project {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		int i, j, temp;
		
		int arr [] = {3,1,4,2,5} ;
		
		for(i=0; i<arr.length; i++) {
		
			temp = arr[i];
			
			for(j=i-1; j>0 && arr[j] > temp; j--)
				arr[j+1] = arr[j];
					arr[j+1] = temp;
						
		}
		
		System.out.println(Arrays.toString(arr));
		
	}
