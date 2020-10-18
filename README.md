# java-10.12
java课件作业项目仓库
1. 基本要求是完成教材P110页的第四题关于PC、HardDisk、CPU类的使用。
2. 每个类定义不少于两个属性，且属性的类型应该多样化;
3. 根据课堂中关于访问权限的内容，尝试定义属性的修饰多样化，类中定义方法操作属性，避免直接通过“类对象属性的形式访问属性值;且定义的方法内应该又符合常理的逻辑判断.
4. 尝试把本次实验的多个类放置在不同的包中，体验修饰符private的用法。
## 2. 实验设计
1.设置硬盘对象，给CPU对象设置amount,speed方法。设置amount,speed方法在硬盘对象外不可访问

   private int speed;		
	private String type;	
	private int ram;

 ## 3. 核心方法
 
    1.

          CPU(int speed,String type,int ram){
		this.speed=speed;
		this.type=type;
		this.ram=ram;
	}
	
	public int getSpeed() {
		return speed;
	}
	public void setSpeed(int speed) {
		this.speed = speed;
	}
	public String getType() {
		return type;
	}
    2.
   
                 CPU cpu = new CPU(2200, "AMD", 32);
		
		HardDisk disk = new HardDisk(459, "西部数据", 500);
   
   
   ## 4. 实验结果
   
   CPU品牌：AMD
  AMD此品牌的CPU为：32位
  CPU运行速度:2200转
-------------------------------
硬盘品牌:西部数据
硬盘价格:459人民币
此品牌硬盘内存大小为：500GB

  ## 5.实验感想

  1. 学到了public private 的不同用法
  2. 学会了如何导出项目，意外中学会了Java类文件放在src根目录下
