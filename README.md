//CSC 142
//Elias Alabssie
// homework #1,chapter 8
 

public class Line {
		private Point startingPoint;
		private Point endingPoint;
		
		
		
	public static void main(String[] args) {
			
		// these snipets of codes are just to see the out put of the methods.
		Point p=new Point (2,4);
		Point p1=new Point (5,6);
		Line l=new Line(2,4,5,6);
			
		System.out.println(l);
		System.out.println(l.getSlop());
		
		
	}
		
		//Line segment constructor
	public Line(Point p1, Point p2){
		this.startingPoint=p1;
		this.endingPoint=p2;
	}
		
			// #14. this method returns the starting point of the line segment object.
	public Point getp1(){
		return startingPoint;
	}
		
		// # 14. this method returns the end point of the line segment object.
	public Point getp2(){
		
		return endingPoint;
		
	}

		// #14.this method returns the string of the line segment object.
	public String toString(){
		
		return "["+"("+startingPoint.getX()+","+startingPoint.getY()+ ")"
					+ ""+","+"("+endingPoint.getX()+","+endingPoint.getY()+")"+"]";

	}
		
		// # 15. this method returns the slope the line segment object.
	public double getSlop(){
		if(endingPoint.getX()==startingPoint.getX()){
			throw new IllegalArgumentException();
		}
		return (double)(endingPoint.getY()-startingPoint.getY())/(endingPoint.getX()-startingPoint.getX());
			
	}
		
		//# 16. this method creates line segment from 4 integers.
	public Line(int x1, int y1, int x2, int y2){
		this(new Point(x1,y1), new Point(x2,y2));
	}
		
}






# CSC-143
This repository stores java codes
