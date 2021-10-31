# Node Ecosystem, TDD, CI/CD

**- Describe (in plain English) what Array.map() does:**  
 The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.

 **- Describe (in plain English) what Array.reduce() does:**  
The reduce() method executes a user-supplied “reducer” callback function on each element of the array, passing in the return value from the calculation on the preceding element. The final result of running the reducer across all elements of the array is a single value.

**- Provide code snippets showing how to use superagent() to fetch data from a URL and log the result:**  

- With normal Promise .then() syntax :

```
  superagent.get('http://swapi.dev/api/people/')
  .then(result=>{
    let dataObject={};
    result.body.results.forEach((item,i)=>{
      dataObject[result.body.results[i].name]=result.body.results[i].homeworld
    })
      console.log(dataObject);
  })
  .catch(err=>{
    console.log(err)
  })
```
- With async / await syntax :

```
async function cityData(cityName){
  let result= await superagent.get(`https://geocode.xyz/${cityName}?json=1`)
  console.log('City Name: '+result.body.standard.city)
  console.log('Longitude: '+result.body.alt.loc.longt)
  console.log('Latitude: '+result.body.alt.loc.latt)

}
cityData('Amman')
```

**- Explain promises as though you were mentoring a Code 301 level student:**  

First we have to know that JavaScript is single threaded, meaning that two bits of script cannot run at the same time; they have to run one after another.
then we can say that a promise is an object that represents the eventual completion (or failure) of an asynchronous operation, and its resulting value.

**- Are all callback functions considered to be Asynchronous? Why or Why Not?**  

No not all functions are asynchronous, the callback will be synchronous when the higher order function which calls it is calling it synchronously. Inversely if it is called within the context of the execution branch of an asynchronous operation it will be asynchronous.
