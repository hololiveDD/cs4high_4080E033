public class Robot {
	int X; 
	int Y; 
	int direction; //機器人 的 前進 方向 N,S,E,W
}
	public Robot() {} 
	
	public Robot(int X,int Y,int direction) {  
	
		this.X=X; 
		this.Y=Y; 
		this.direction=direction; 
	}
	
	public int getX() {
		return X; 
	}
	
	public int getY() { 
		return Y; 
	}
	
	public int getdirection() {
		return direction; 
	}
	
	public void setX(int X) {
		this.X=X; 
	}
	
	public void setY(int Y) {
		this.Y=Y; 
	}
	
	public void setdirection(int direction) {
		this.direction=direction; 
	}
	
	public void printRobot() {
		System.out.println(X+"\n"+Y+"\n"+direction+"\n");
	}
	
	public static void main(String[] args) {
		Robot obj_r1 = new Robot(0,3,'S'); 
		obj_r1.printRobot(); 
		
		Robot obj_r2 = new Robot(0,0,'N'); 
		obj_r2.printRobot(); 
		
		Robot obj_r3 = new Robot(2,5,'W'); 
		obj_r3.printRobot(); 
		
		obj_r3.setY(3); 
		obj_r3.printRobot(); 
		System.out.println(obj_r3.direction);
		} //end of main method
} //end of class
