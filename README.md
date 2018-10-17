# ThePennyPantry
function init() {
 Tabletop.init( { key: ‘https://docs.google.com/spreadsheets/d/18eF2tRLO8yrySY9KJWZeeUo6xGoT48hpXLjcoOdCrDo/pubhtml',
 callback: function(data, tabletop) { 
 console.log(data)
 },
 simpleSheet: true } )
 }
function showInfo(data, tabletop) {
console.log(data);
for (var i = 0; i < data.length; i++) {
$(‘.post’).append(
‘<div class=”article” style=”background-image: url( ‘ +
data[i].img + ‘.jpg)”>’ +
‘<div class=”text”>’ +
‘<h1>’ + data[i].Special Name + ‘</h1>’+
data[i].body +
‘</div> ‘ + ‘<div class=”meta-info”>’ + ‘<img src =”’ + data[i].img + ‘.jpg”>’+
‘<div class=”date”>’ + data[i].date + ‘</div>’ +
‘</div>’ +
‘</div>’);
}
}
window.addEventListener(‘DOMContentLoaded’, init)

