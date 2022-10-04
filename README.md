public class Main {
    public static void main(String[] args) {


        try {
            System.out.println("divide 1/0");
            int x = 1 / 0;
            System.out.println(x);
            int[] y = {1, 2, 3};
            System.out.println("reference an index outside of the index range");
            System.out.println(y[4]);


        } catch (ArithmeticException e) {
            //the error is catch here
            System.out.println("This is why QA Engineers always have to do boundary testing! The array has only " +
                    "3 values and you've requested a 4th");

        }
    }
}
