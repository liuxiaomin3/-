# learn-demo
package j26_ch5;

import java.util.Scanner;

public class exc {
	public static void main(String[] args) {
		
		System.out.println("Myshopping管理系统");
		System.out.println("========================");
		System.out.println("1.客户信息管理");
		System.out.println("2.购物结算");
		System.out.println("3.真情回馈");
		System.out.println("4.注销");
		System.out.println("========================");
		
		boolean isRight=false;
		do{
			Scanner input=new Scanner(System.in);
      //注意进行二次循环时，input.hasNextInt()的值始终是false,所以创建Scanner对象要放在do-while循环里面
			int choice=0;
			System.out.println("请选择，输入数字：");
			if(input.hasNextInt()){
				choice=input.nextInt();
			}
			switch(choice){
			case 1:
				isRight=true;
				break;
				
			case 2:
				isRight=true;
				break;
				
			case 3:
				isRight=true;
				break;
				
			case 4:
				isRight=true;
				break;
				
			default:
				isRight=false;
				
				break;
			}
			
		}while(isRight==false);
		
	}
}

