public class MyClass {
    public static void main(String args[]) {
        System.out.println("Hi");
        ChildClass cc = new ChildClass(25,45);
        System.out.println(cc.getAge());
        System.out.println(cc.getID());
        
        ParentClass pc = new ParentClass(88);
        System.out.println(pc.getAge());
    }
}

class ParentClass{
    int age;
    ParentClass(){
        
    }
    ParentClass(int age){
        this.age = age;
    }
    public int getAge(){
        return this.age;
    }
}
class ChildClass extends ParentClass{
    //int age;
    int ID;
    ChildClass(int age, int ID){
        //super(age);
        this.age = age;
        this.ID = ID;
    }
    public int getAge(){
        return this.age;
    }
    public int getID(){
        return this.ID;
    }
}
