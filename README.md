package binaryproject;

public class array2D {

	//public static void main(String[] args) {
	public static void bubbleSort(int[] arr) {
        int n = arr.length;
        for (int i = 0; i < n-1; i++) {
            boolean sorted = true;
            for (int j = 0; j < n-i-1; j++) {
                if (arr[j] > arr[j+1]) {
                    int temp = arr[j];
                    arr[j] = arr[j+1];
                    arr[j+1] = temp;
                    sorted = false;
                }
            }
            if (sorted) {
                break;
            }
        }
    }
  
    public static void main(String[] args) {
        int[] arr = {64, 34, 25, 12, 22, 11, 90};
        bubbleSort(arr);
        System.out.println(arr);
    
}
//In this code, the bubbleSort method takes an integer array arr as input and sorts it using the bubble sort algorithm. The main method tests the sorting algorithm by creating an array of integers and calling the bubbleSort method on it. The sorted array is then printed to the console.





		

	}


