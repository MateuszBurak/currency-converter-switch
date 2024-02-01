# Mateusz Burak - simple currency converter using *input*

## Homepage and portfolio

This project is a part of my learning process of becomming a Frontend developer. You can check the main homepage below.

[Link to the homepage](https://mateuszburak.github.io/Public-homepage/) |
[Link to the homepage's repository](https://github.com/MateuszBurak/Public-homepage)

## Currency converter - input - April 29th, 2023

[Link to the converter](https://mateuszburak.github.io/currency-converter-input/) |
[Link to the converter's repository](https://github.com/MateuszBurak/currency-converter-input)

This simple converter does not use api, as it's mostly meant to practice the *input* element

```javascript
formElement.addEventListener("input", () => {

    let amount = amountElement.value;
    let currency = currencyElement.value;
    let result = resultElement.value;

    let currencyEUR = 4.63;
    let currencyUSD = 4.16;
    let currencyGBP = 5.23;

    switch (currency) {
        case "EUR":
            result = amount / currencyEUR;
            signElement.innerText = " €";
            break;
        case "USD":
            result = amount / currencyUSD;
            signElement.innerText = " $";
            break;
        case "GBP":
            result = amount / currencyGBP;
            signElement.innerText = " £";
            break;
    }

    resultElement.innerText = result.toFixed(2);
})
```