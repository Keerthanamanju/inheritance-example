# inheritance-example
package shapeinheritanceexample;
abstract class Shape {
public abstract double calculateArea();
}
class Circle extends Shape{
private double radius;
public Circle(double radius) {
this.radius = radius;
}
public double calculateArea() {
return Math.PI * radius * radius;
}
}
class Rectangle extends Shape {
private double length, width;
public Rectangle(double length, double width) {
this.length = length;
this.width = width;
}
public double calculateArea() {
return length * width;
}
}
class Square extends Shape {
private double side;
public Square(double side) {
this.side = side;
}
public double calculateArea() {
return side * side;
}
}
class Triangle extends Shape {
private double base,height;
public Triangle(double base, double height) {
this.base = base;
this.height = height;
}
public double calculateArea() {
return 0.5 * base * height;
}
}
/**
 *
 * @author 1BSCCSA47
 */
public class ShapeInheritanceExample {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
         Shape Circle = new Circle(5);
        Shape  Rectangle = new Rectangle(4, 6);
        Shape square = new Square(4);
        Shape Triangle = new Triangle(3, 5);
    
        System.out.println("circle area:"+Circle.calculateArea());
        System.out.println("rectangle area:"+Rectangle.calculateArea());
        System.out.println("Square Area:"  + square.calculateArea());
        System.out.println("Triangle Area:"  + Triangle.calculateArea());
       
 
    
    }
    
}
run:
Addition of two integers: 999
Addition of three integers: 1332
Addition of two doubles: 30.369999999999997
BUILD SUCCESSFUL (total time: 0 seconds)
