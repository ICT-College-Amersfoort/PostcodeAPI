# PostcodeAPI
Postcode API, een lichtgewicht jQuery Plugin om de webservice postcodeapi.nu te integreren via jQuery (http://api.postcodeapi.nu/docs/)
Er is een probleem met het checken van de postcode in combinatie met het huisnummer. Volgens de voorbeelden moet dat mogelijk zijn, op http://boye.e-sites.nl/papi/ werkt dit ook.
Zodra ik dit in een eigen omgeving probeer, lukt het niet om een verkeerd huisnummer bij een postcode GEEN output te laten genereren! Met andere woorden, de straatnaam en adres worden gewoon ingevuld.

$('#housenr').papi({
    source: $('#zipcode4')[0],
    event: 'change',
    placeholders: {
        street: $('#street4')[0],
        town: $('#town4')[0]
    }
});
