# Java_me





public abstract class Animals {


 //    public  abstract void paws();
 
    public static void main(String[] args) {
        Dog dog = new Dog();
        Cat cat = new Cat();

        dog.setColor ("я коричневого кольору " + "("+ "brown" +")" );
        dog.setName("Привіт я " + "Ведмідь бурий");

        cat.setColor("I brown");
        cat.setName("Barsik is me");
        System.out.println(dog.getName());
        System.out.println(dog.getColor());

        System.out.println(cat.getName());
        System.out.println(cat.getColor());
    }
    public abstract void paws();

}

// class Cat extends Animals{
  //  private String name = "Барсік";
 //   public void speak(){

 //   }

  //   public final void paws(){
   //      System.out.println("Привіт я " + name);
   //  }
//}

// class Dog extends Animals{
 //    private String name;
 //    public void speak(){

 //   }

 //   public final void paws(){

 //           System.out.println("У мене чотири лапи ");
 //   }
//}




 class Dog extends Animals {
     private String name;
     private String color;


     public String getName() {
         return name;
     }

     public  void setName(String name) {
         this.name = name;
     }

     public String getColor() {
         return color;
     }

     public final void paws(){
         System.out.println("У мене чотири лапи ");
     }
     public final void setColor(String color) {
         this.color = color;
     }

 }


     class Cat extends Animals {
         private String name;
         private String color;



         public String getName() {
             return name;
         }

         public void setName(String name) {
             this.name = name;
         }

         public String getColor() {
             return color;
         }
         public final void paws(){

         }

         public final void setColor(String color) {
             this.color = color;
         }

     }







