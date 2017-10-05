import java.util.Scanner;

public class faiz
{

	static Scanner Scan = new Scanner (System.in);

	public static void main (String[] args)
	{

		int sene;
		double faiz, sonuc,borc;

		System.out.print ("Borç: ");
		borc = Scan.nextDouble ();

		System.out.print ("Faiz Oranı: ");
		faiz = Scan.nextDouble ();

		System.out.print ("Sene: ");
		sene = Scan.nextInt ();

		sonuc = (borc + (((borc * faiz) / 100) *  sene));

		System.out.println (
				"Borcunuz: " + sonuc + ", Aylık ödemeniz: " +
				String.format ("%.2f", (sonuc / (sene * 12))) + "."
		);

	}

}
