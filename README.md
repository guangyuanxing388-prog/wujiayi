public class Test {

    public static void main(String[] args) {

        Animal dog = new Dog();
        Animal bird = new Bird();

        System.out.println("=== 测试 Dog（Animal 类型）===");
        dog.eat();
        dog.move();
        dog.sleep();

        System.out.println("\n=== 测试 Bird（Animal 类型）===");
        bird.eat();
        bird.move();
        bird.sleep();

        System.out.println("\n=== 测试 Dog 的 swim() ===");
        Swimable swimableDog = new Dog();
        swimableDog.swim();

        ((Dog) dog).swim();
    }
}
