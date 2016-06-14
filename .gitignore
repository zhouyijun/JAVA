package oop06;

/*
 * 编写 电话 移动电话  固定电话 体现三者之间的继承关系
     电话  包含 属性：品牌，号码
                方法：打电话  接电话
     手机  
              重写父类中  打  电话接电话
方法 ：接收短信
     固定电话  
			  重写父类中  打电话  接电话
			  方法：接宽带
     电话厂：
         方法：测试电话   testPhone(Phone  p) ,能在方法内调用电话的打电话与接电话方法
               生产电话   getPhone(int type)
               当 type 为1 则生成一个固定电话
                  Type为2 则生成一个手机
				  其他 则生成一个 电话
				××注意考虑该方法的返回类型××
 */
public class Phone {
	String brand;
	int number;
	
	public void hit(){
		System.out.println("打电话！");
	}
	public void join(){
		System.out.println("接电话！");
	}
	public void yield(){
		System.out.println("生成一个电话！");
	}
}

class Mobile extends Phone{
	public void hit(){
		System.out.println("打手机电话！");
	}
	public void join(){
		System.out.println("接手机电话！");
	}
	public void yield(){
		System.out.println("生成一个手机！");
	}
}
class Fixed extends Phone{
	public void hit(){
		System.out.println("打固定电话！");
	}
	public void join(){
		System.out.println("接固定电话！");
	}
	public void yield(){
		System.out.println("生成一个固定电话！");
	}
}

class TestPhone {
	public void Test(Phone p){
		p.hit();
		p.join();
		p.yield();
	}
	public Phone getPhone(int type){
		if(type==1){
			return  new Fixed();
		}else if(type==2){
			return  new Mobile();
		}else{
			return  new Phone();
		}
	}
	public static void main(String[] args){
		TestPhone ps = new TestPhone();
//		Phone p = new Phone();
//		ps.Test(p);
		Phone p1=ps.getPhone(1);
		Phone p2=ps.getPhone(2);
		Phone p3=ps.getPhone(3);
		p1.yield();
		p2.yield();
		p3.yield();
	}}





