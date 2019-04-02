import.java.io.*;
package pkgShape;
public abstract class Shape {
	   public abstract double area();
	   public abstract double paremeter();
	   
}
public class Rectangle extends Shape{
	private int width;
	private int length;
	
	
	public int setWidth(int) {
         if(int < 1) { 
			throw new IllegalArgumentException("width must be positive");
		}else {
			int = width;
		}
		}
	public int setLength(int) {
		if(int < 1) { 
			throw new IllegalArgumentException("length must be positive");
		}else {
			int = length;
		}
		}
	}
    public int getWidth() {
    	return width;
    }
    public int getLength() {
    	return length;
    }
	public double area(length, width) {
		area = length*width;
	}
	public double parameter(length, width) {
		parameter = (2*length)+(2*width);
	}


public class Cuboid extends Rectangle{
	private int depth;
	
	public int setDepth(int a) {
        if(a < 1) { 
			throw new IllegalArgumentException("depth must be positive");
		}else {
			a = depth;
		}
		}
	public int getDepth(){
		return depth;
	}
	
	public double volume(length,width,depth){
		int volume = length*width*depth;
	}
	public double parameter() {
		throw new UnsupportedOperationException("we don't do dat here");
	}
	@Override
	public double area(length, width, depth) {
		area = (2*(length*width))+(2*(length*depth))+(2*(depth*width));
	}
}
