Lab Assignment 02 : Javascript (section : 06)
You have to prepare an online currency converter. The description of which is given in the PDF file



const USD = document.getElementById('usd');

const GBP = document.getElementById('gbp');

const CAD = document.getElementById('cad');

const EUR = document.getElementById('eur');

const AUD = document.getElementById('aud');



usd.addEventListener('input', usdToGbpToCadToEurToAud);

function usdToGbpToCadToEurToAud(){

 const ud = parseFloat(usd.value);

 const gp = 0.80*ud;

 const cd = 1.36*ud;

 const eu = 0.89*ud;

 const ad = 1.45*ud;

 gbp.value = gp;

 cad.value = cd;

 eur.value = eu;

 aud.value = ad;



}



usdToGbpToCadToEurToAud()

gbp.addEventListener('input', gbpToUsdToCadToEurToAud);

function gbpToUsdToCadToEurToAud(){

	const gp = parseFloat(gbp.value)

	const ud = 1.25*gp;

	const cd = 1.70*gp;

	const eu = 1.11*gp;

	const ad = 1.81*gp;

	usd.value = ud;

	cad.value = cd;

    eur.value = eu;

    aud.value = ad;

}

cad.addEventListener('input', cadToUsdToGbpToEurToAud);

function cadToUsdToGbpToEurToAud() {

	const cd = parseFloat(cad.value)

	const ud = 0.74*cd;

	const gp = 0.59*cd;

	const eu = 0.65*cd;

	const ad = 1.07*cd;

	usd.value = ud;

	gbp.value = gp;

    eur.value = eu;

    aud.value = ad;

}

eur.addEventListener('input', eurToUsdToGbpTocadToAud);

function eurToUsdToGbpTocadToAud() {

	const eu = parseFloat(eur.value)

	const ud = 1.13*eu;

	const gp = 0.90*eu;

	const cd = 1.53*eu;

	const ad = 1.63*eu;

	usd.value = ud;

	gbp.value = gp;

    cad.value = cd;

    aud.value = ad;

}

aud.addEventListener('input', audToUsdToGbpTocadToEur);

function audToUsdToGbpTocadToEur() {

	const ad = parseFloat(aud.value)

	const ud = 0.69*ad;

	const gp = 0.55*ad;

	const cd = 0.94*ad;

	const eu = 0.61*ad;

	usd.value = ud;

	gbp.value = gp;

    cad.value = cd;

    eur.value = eu;

}

Show more...



const USD = document.getElementById('usd');

const GBP = document.getElementById('gbp');

const CAD = document.getElementById('cad');

const EUR = document.getElementById('eur');

const AUD = document.getElementById('aud');



usd.addEventListener('input', usdToGbpToCadToEurToAud);

function usdToGbpToCadToEurToAud(){

 const ud = parseFloat(usd.value);

 const gp = 0.80*ud;

 const cd = 1.36*ud;

 const eu = 0.89*ud;

 const ad = 1.45*ud;

 gbp.value = gp;

 cad.value = cd;

 eur.value = eu;

 aud.value = ad;



}



usdToGbpToCadToEurToAud()

gbp.addEventListener('input', gbpToUsdToCadToEurToAud);

function gbpToUsdToCadToEurToAud(){

	const gp = parseFloat(gbp.value)

	const ud = 1.25*gp;

	const cd = 1.70*gp;

	const eu = 1.11*gp;

	const ad = 1.81*gp;

	usd.value = ud;

	cad.value = cd;

    eur.value = eu;

    aud.value = ad;

}

cad.addEventListener('input', cadToUsdToGbpToEurToAud);

function cadToUsdToGbpToEurToAud() {

	const cd = parseFloat(cad.value)

	const ud = 0.74*cd;

	const gp = 0.59*cd;

	const eu = 0.65*cd;

	const ad = 1.07*cd;

	usd.value = ud;

	gbp.value = gp;

    eur.value = eu;

    aud.value = ad;

}

eur.addEventListener('input', eurToUsdToGbpTocadToAud);

function eurToUsdToGbpTocadToAud() {

	const eu = parseFloat(eur.value)

	const ud = 1.13*eu;

	const gp = 0.90*eu;

	const cd = 1.53*eu;

	const ad = 1.63*eu;

	usd.value = ud;

	gbp.value = gp;

    cad.value = cd;

    aud.value = ad;

}

aud.addEventListener('input', audToUsdToGbpTocadToEur);

function audToUsdToGbpTocadToEur() {

	const ad = parseFloat(aud.value)

	const ud = 0.69*ad;

	const gp = 0.55*ad;

	const cd = 0.94*ad;

	const eu = 0.61*ad;

	usd.value = ud;

	gbp.value = gp;

    cad.value = cd;

    eur.value = eu;

}
