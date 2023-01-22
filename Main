import java.util.*;  
class UserInput{
    public void get(double[] dist, double[] time)
        {
            Scanner sc=new Scanner(System.in); 
            System.out.println("Enter distance for first 10 vehicles in kilometer");
            for(int i = 0; i < 10; i++)
            {
                dist[i] =sc.nextDouble() ;
            }
            System.out.println("Enter time taken to cover the first 10 distance in hour");
            for (int i = 0; i < 10; i++)
            {
                time[i] = sc.nextDouble() ;
            }
        }
}
class Measure extends UserInput
{
    public void calculate_speed(double[] dist, double[] time, double[] speed)
        {
            for(int i = 0; i < 10; i++)
            {
                speed[i] = (dist[i]*1000) / (time[i]*60);
            }
        }
}
class ShowResults extends Measure
{
    public void Display(double[] dist, double[] time, double[] speed)
        {
            System.out.println("Distance      Time      Speed");
            for(int i = 0; i < 10; i++)
            {
                System.out.println(dist[i] +" KM       "+ time[i]+" hrs      " + speed[i]+" m/s");
            }
        }
}
class Main {
    public static void main(String[] args) {
        double[] dist = new double[10];
        double[] time = new double[10];
        double[] speed = new double[10];
        ShowResults obj = new ShowResults();
        obj.get(dist,time);
        obj.calculate_speed(dist, time, speed);
        obj.Display(dist,time,speed);
    }
}
