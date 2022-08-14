# linear_Search
Java program for linear search(Approach 01) along with its theory.

class Practise
{
 
    public static int  linear_search(int arr[], int key) {
        int n =arr.length;
        for(int i =0;i<n;i++)
        {//Check if current element matches with the key 
         if(arr[i]==key)
         {
             return i ;
         }
        } 
        //out of the loop 
        return -1;
     }

     public static void main(String args[])
    {
        int arr[]={2,3,5,7,6,8,9,45,23,44,66,65,89};
        int key = 44;
        //function call
        int result = linear_search(arr, key);
        if (result == -1)
        {
            System.out.println("Key is not present in the array ");

        }
        else
        {
            System.out.println("Key is present at index"+ result );
        }




    }
    
}

    

//Java program for linear search(Approach 02) along with its theory.


// Java program for linear search

import java.io.*;

class GFG
{

	public static void search(int arr[], int search_Element)
	{
		int left = 0;
		int length = arr.length;
		int right = length - 1;
		int position = -1;

		// run loop from 0 to right
		for (left = 0; left <= right;)
		{
			
			// if search_element is found with left variable
			if (arr[left] == search_Element)
			{
				position = left;
				System.out.println(
					"Element found in Array at "
					+ (position + 1) + " Position with "
					+ (left + 1) + " Attempt");
				break;
			}
		
			// if search_element is found with right variable
			if (arr[right] == search_Element)
			{
				position = right;
				System.out.println(
					"Element found in Array at "
					+ (position + 1) + " Position with "
					+ (length - right) + " Attempt");
				break;
			}
			
			left++;
			right--;
		}

		// if element not found
		if (position == -1)
			System.out.println("Not found in Array with "
							+ left + " Attempt");
	}

	
	// Driver code
	public static void main(String[] args)
	{
		int arr[] = { 1, 2, 3, 4, 5 };
		int search_element = 5;
	
		// Function call
		search(arr,search_element);
	}
}
























