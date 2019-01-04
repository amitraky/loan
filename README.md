## Plan


# RD calculator
```
n = term_in Months / 12;


CP =   P + ((P*r*n)/100);


P = 1200
r = 3.8333
n = 12/12

A = 1200 + (1200*3.8333*1)/100;
A = 1200 + 45.9996;
A = 1245.9996 ;
```

# Loan compund

```
 A = P * r (1+r) / ( (1+r) ^ n  - 1))  
```

# Loan Flat
```
function doFlatRateCalculation(L, r, n) {
	// L is loan amount
	// r is flat rate
	// n is number of months
	
	T =  (1 + (n * r/1200)) * L;
	P = T/n;
	console.log(P);
	return P;
}
```
# Compount 
```

function doCompoundCalculation(L, r, n) {
	// L is loan amount
	// r is APR
	// n is number of months

	P = L * r * Math.pow(1+r/1200,n) / (1200 * (Math.pow(1+r/1200,n) - 1));
	return P;
}
```
