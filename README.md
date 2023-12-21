public class MyNumber {
    private int value;

    public MyNumber(int value) {
        this.value = value;
    }

    // Overloading the '+' operator
    public MyNumber add(MyNumber other) {
        int result = this.value + other.value;
        return new MyNumber(result);
    }

    public void display() {
        System.out.println("Value: " + value);
    }

    public static void main(String[] args) {
        MyNumber num1 = new MyNumber(5);
        MyNumber num2 = new MyNumber(10);

        MyNumber sum = num1.add(num2);

        System.out.print("num1: ");
        num1.display();

        System.out.print("num2: ");
        num2.display();

        System.out.print("Sum: ");
        sum.display();
    }
}
