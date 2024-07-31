const getWeather = (cityName) => {
    const fetchWeather = fetch(
    'https://api.openweathermap.org/data/2.5/weather?
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
