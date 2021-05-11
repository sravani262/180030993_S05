package Array;

public class twentynine {

	public static void main(String[] args) {
		int a[][]=new int[3][3];
		int n=0;
		for(int i=0;i<3;i++)
		{
			for(int j=0;j<3;j++)
			{
				a[i][j]=Integer.parseInt(args[n]);
				n++;
			}
		}
		if(args.length!=9)
		{
			System.out.print("Please enter 9 integer numbers");
			return;
		}
		int max=a[0][0];
		for(int i=0;i<3;i++)
		{
			for(int j=0;j<3;j++)
			{
				if(a[i][j]>max)
				{
					max=a[i][j];
				}
			}
		}
		System.out.print(max);
	}
}
