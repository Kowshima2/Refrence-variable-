# Refrence-variable-
class Car {
    
    String brand;
    int year;

   
    Car(String brand, int year) {
        this.brand = brand;
        this.year = year;
    }

    void display() {
        System.out.println("Brand: " + brand);
        System.out.println("Year: " + year);
    }
}

public class ReferenceVariableExample {
    public static void main(String[] args) {
        Car myCar = new Car("Toyota", 2021);
        myCar.display();
        Car yourCar = myCar;  
        yourCar.brand = "Honda";
        
      
        System.out.println("\nDetails of myCar after modification:");
        myCar.display();  

        System.out.println("\nDetails of yourCar:");
        yourCar.display();
    }
}

Output 

Brand: Toyota
Year: 2021

Details of myCar after modification:
Brand: Honda
Year: 2021

Details of yourCar:
Brand: Honda
Year: 2021
