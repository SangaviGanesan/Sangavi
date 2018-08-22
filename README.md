//lowest millage car
import java.util.*;
public class Hello {
    public static void main(String[] args) {
        float x,y=100000;
        int i;
        String s,u="",a[];
        Scanner sc=new Scanner(System.in);
        s=sc.nextLine();
        a=s.split(" ");
        String[] b=new String[10];
        for(i=0;i<a.length;i++)
        {
            b=a[i].split("@");
            x=Float.parseFloat(b[1]);
            if(x<y){
                u=b[0];
                y=x;
            }
        }
        System.out.println(u);
    }
}
