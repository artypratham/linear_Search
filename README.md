# linear_Search
Java program for linear search along with its theory.
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

    




























