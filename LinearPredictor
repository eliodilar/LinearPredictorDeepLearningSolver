//import java.math.*;

public class PredicateurLineaire {
	
	
	public static void main(String arg[]){
		
		int Cpt = 0;
		double douzetrenhuitEuro = 12.38;
		double DixSeptTrenteTroisDollars = 17.33;
		double Result = 1.0;
		double Coefficient = 0.0;
		boolean LowFlag = false;
		boolean PosFlag = false;

		System.out.println("----------------------------------------");
		System.out.println("linear predictor running:" );
		System.out.println("----------------------------------------");
		System.out.println(" ");
		
		Coefficient = (douzetrenhuitEuro + DixSeptTrenteTroisDollars ) / 2;
		
		while (PosFlag == false || LowFlag == false){
				
			Result = Coefficient * douzetrenhuitEuro;
				
			if (Result > DixSeptTrenteTroisDollars){
				
				Coefficient -= 0.001;
				
				PosFlag = true;
				
			}
			else if(Coefficient < DixSeptTrenteTroisDollars){
				
				Coefficient += 0.001;
				
				LowFlag = true;
					
			}
				
			System.out.println("Cpt :" +  Cpt++ + "  - Coefficient = "  + Coefficient);
 				
		}
		
		Result = Coefficient * douzetrenhuitEuro;
			
		System.out.println(" ");
		System.out.println("----------------------------------------");
		System.out.println("The good coefficient is :" +  Coefficient);
		System.out.println("----------------------------------------");
		System.out.println(" ");
		System.out.println("The result of coef * euros t is :" +  Result);
		
		if ( Result > DixSeptTrenteTroisDollars){
			
			System.out.println("The margin error is of :" +  Math.abs(((DixSeptTrenteTroisDollars/Result) * 100) - 100) + "%");
			
		}
		else{
			
			System.out.println("The margin error is of :" +  Math.abs(((Result/DixSeptTrenteTroisDollars) * 100) - 100) + "%");
			
		}

	}
	
}
