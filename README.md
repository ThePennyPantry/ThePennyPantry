# ThePennyPantry
function init() {
 Tabletop.init( { key: ‘https://docs.google.com/spreadsheets/d/18eF2tRLO8yrySY9KJWZeeUo6xGoT48hpXLjcoOdCrDo/pubhtml',
 callback: function(data, tabletop) { 
 console.log(data)
 },
 simpleSheet: true } )
}
window.addEventListener(‘DOMContentLoaded’, init)
