# VEF2B3U Lokaverkefni

## Um verkefnið

Þetta er lokaverkefnið mitt, Guðna Natans Gunnarssonar, í áfanganum VEF2B3U. Verkefnið er síða sem sækir sjálfkrafa upplýsingar um tónleika sem verða á næsta leiti. Hægt er að leita að sérstökum tónleikum, eða flokka þá eftir staðsetningu. Vefsíðan styður alla betri vafra og allar skjástærðir.


## Kóða sýnidæmi

Hérna er kóðinn sem sækir tónleikaupplýsingarnar frá [apis.is](http://docs.apis.is/#endpoint-concerts):
~~~~
$.ajax({
	'url': 'http://apis.is/concerts/',
	'type': 'GET',
	'dataType': 'json',
	'success': function(response) {
	  	concertSuccess(response);
	},
	'error': function(response){
	  	concertError(response);
	}
});
~~~~

## Notkun

Hægt er að prófa vefsíðuna með því að fylgja þessari slóð:
[http://tsuts.tskoli.is/2t/1803982879/VEF2B3U/Lokaverkefni/](http://tsuts.tskoli.is/2t/1803982879/VEF2B3U/Lokaverkefni/)


## API

Þetta verkefni notar API frá apis.is.
Hægt er að finna hann á vefsíðu [apis.is](http://docs.apis.is/#endpoint-concerts).

## Gert af

Guðni Natan Gunnarsson, 2017.

## License

Copyright (c) <2017> <Guðni Natan Gunnarsson>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.