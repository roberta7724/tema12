package tema12;

import java.util.ArrayList;

public class Array {

	public static void main(String[] args) {
		
		 ArrayList<String> list1 = new ArrayList<String>();
	        list1.add("hello");
	        list1.add("world");
	        System.out.println("Before Swap: " + list1);
	        swapFirstLast(list1);
	        System.out.println("After Swap: " + list1);

	        ArrayList<String> list2 = new ArrayList<String>();
	        list2.add("hello");
	        System.out.println("\nBefore Swap: " + list2);
	        swapFirstLast(list2);
	        System.out.println("After Swap: " + list2);

	        ArrayList<String> list3 = new ArrayList<String>();
	        System.out.println("\nBefore Swap: " + list3);
	        swapFirstLast(list3);
	        System.out.println("After Swap: " + list3);
	}
	 public static void swapFirstLast(ArrayList<String> list) {
	        if (list.size() > 1) {
	            list.add(0, list.remove(list.size() - 1));
	            list.add(list.size(), list.remove(1));
	        }
	    }
	
	
}

