public class Main {
    public static void main(String[] args) {
        int[] myarr = {0, 2, 3, 5, 6, 6};
        System.out.println("The count of even numbers is  " + countEvenNumbers(myarr, 0));


    }

    public static int countEvenNumbers(int[] arr, int idx) {
        if (arr.length == 0 || idx == arr.length) return 0;


        return ((arr[idx] % 2 == 0)?  countEvenNumbers(arr, idx + 1) + 1 : countEvenNumbers(arr, idx + 1));



    }

}
