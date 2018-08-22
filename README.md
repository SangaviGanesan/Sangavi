//small matrix

import java.util.*;
class Main{
public static void main (String[] args) {
    
Scanner sc=new Scanner(System.in);
int i,j,x=0,y=0,count=0;
    int n,m,flag=0;
    n=sc.nextInt();
    m=sc.nextInt();
    int a[][]=new int[n][n],b[][]=new int[n][n];
    for(i=0;i<n;i++)
        for(j=0;j<n;j++)
            //cin>>a[i][j];
            a[i][j]=sc.nextInt();
    for(i=0;i<m;i++)
        for(j=0;j<m;j++)
            //cin>>b[i][j];
            b[i][j]=sc.nextInt();
    for(i=0;i<n;i++)
    {
        for(j=0;j<n;j++)
        {
            if(a[i][j]==b[x][y])
            {
                count++;
       
                if(y<m)
                    y++;
                if(y>=m)
                    {
                        x++;
                        y=0;
                    }
                if(count==m*m)
                    flag=1;
                
            }
        }
    }    
        
    if(flag==1)
        System.out.println("TRUE");
    else
        System.out.println("FALSE");
 }
}
