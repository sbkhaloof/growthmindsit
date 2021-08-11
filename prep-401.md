# Node Ecosystem, TDD, CI/CD
## Review, Research, and Discussion
### Describe (in plain English) what Array.map() does
##### The array.map() function iterates over an array and runs a call back for each element. it will always return you a new array of the same length as the original array comprised of your return values .


-------------------------------------------------
### Describe (in plain English) what Array.reduce() does

##### The reduce() method executes a reducer function (that you provide) on each element of the array, resulting in a single output value .

-------------------------------------------------
### Provide code snippets showing how to use superagent() to fetch data from a URL and log the result
1. With normal Promise .then() syntax :
#### function getWeatherInfoHandler(req,res){
let findQuery=req.query.cityName;
let weatherUrl=`https://api.weatherbit.io/v2.0/forecast/daily?city=${findQuery}&key=${process.env.WEATHER_API_KEY}`
axios
.get(weatherUrl)
.then(weatherData=>
     {
       let wData=weatherData.data.data.map(city=>{
       return new Forecast(city.valid_date,city.weather.description)
     })
res.send(wData)

 })


2. Again with async / await syntax
#### getWeatherData = async () => {
    let city = this.state.findQuery.charAt(0).toUpperCase() + this.state.findQuery.slice(1); 
    let weatherUrl = `https://city-explorer-api-backend.herokuapp.com/getWeatherInfo?cityName=${city}&format=json`;
     let weather = await axios.get(weatherUrl);
    await this.setState({
      weatherArr:weather.data,
      showWeather:true,
      })
  }
-----------------------------------------------
### Explain promises as though you were mentoring a Code 301 level student
#### A Promise is an object that represents the eventual completion (or failure) of an asynchronous operation, and its resulting value.The Promise object works as proxy for a value not necessarily known when the promise is created. It allows you to associate handlers with an asynchronous action’s eventual success value or failure reason.This lets asynchronous methods return values like synchronous methods: instead of immediately returning the final value, the asynchronous method returns a promise to supply the value at some point in the future.

-----------------------------------------------
### Are all callback functions considered to be Asynchronous? Why or Why Not?
#### Argument function can be called synchronously(Simply taking a callback doesn't make a function asynchronous. There are many examples of functions that take a function argument but are not asynchronous. For example there's forEach in Array. It iterates over each item and calls the function once per item),also Asynchronous function needs to perform an asynchronous operation ; For a function to be asynchronous it needs to perform an asynchronous operation. It needs to incorporate the argument callback in handling the results of this asynchronous operation. Only this way the function becomes asynchronous.

[Home Page](https://sbkhaloof.github.io/growthmindsit/readme)