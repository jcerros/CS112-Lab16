public class RandomNumberMain {
        public static void main(String args[]){
            
            RandomNumber object= new RandomNumber(1,10);
            RandomNumber object2= new RandomNumber(1,20);

            RandomNumber object3= new RandomNumber(1,30);

            
            System.out.println(object.GetANumber());
            System.out.println(object2.GetANumber());
            System.out.println(object3.GetANumber());
        }
    }

public class RandomNumber {
    int lo, high;

    public RandomNumber(int LoBound, int Highbound) {
        lo = LoBound;
        high = Highbound;
    }

    public int GetANumber_Between_1_and_10() {

        return 1 + (int) (Math.random() * 10);
    }

    public int GetANumber(int lo, int high) {

        return lo + (int) (Math.random() * high);

    }

    public int GetANumber() {
        
        return lo + (int) (Math.random() * high);

    }

}
