# Run-time-polymorphism


Coding-

package runtimepolymorphism;
class Shape {
    public void draw() {
        System.out.println("Drawing a shape");
    }
}

class Circle extends Shape {
    @Override
    public void draw() {
        System.out.println("Drawing a circle");
    }
}

class Rectangle extends Shape {
    @Override
    public void draw() {
        System.out.println("Drawing a rectangle");
    }
}

public class ShapeTest {
    public static void main(String[] args) {
        
        Shape shape;

        // Assigning Circle object to Shape reference
        shape = new Circle();
        shape.draw();  // Output: Drawing a circle

        // Assigning Rectangle object to Shape reference
        shape = new Rectangle();
        shape.draw();  
    }
}



Output-

Drawing a circle
Drawing a rectangle
