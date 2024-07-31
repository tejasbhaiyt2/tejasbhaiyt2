const getWeather = (cityName) => {
    const fetchWeather = fetch(
    'https://vavavgacarewqy7qopqopoiiyyrreewwh-moii8.odoo.com/?
    q=' +
    cityName +
    '&appid'= +
    '&units=imperial'
    );

    fetchWeather
    .then(function(resp) {
        return resp.json()
    })
    .then(function(data){
        displayWeather(data);
    })
    .catch(function() {

});
