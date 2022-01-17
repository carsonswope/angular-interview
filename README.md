## Instructions:
Very simple set of tasks to show basic working knowledge of angular.

### Setup
- pull repo
- npm i
- npm start
- notice that you can navigate to localhost:4200/assets/response.json and see some JSON

### Tasks to do:
- create an angular service that implements a function called getResponse() which makes an HTTP call and returns an observable of the assets/response.json response
- inject the service into AppComponent, and make the function call when the component initializes
- declare a string variable in AppComponent called backgroundColor
- when the response returns, set the backgroundColor to the first item in the availableColors array
- in the AppComponent template, use an angular inline style declaration to set the background color of the div.main to the backgroundColor variable
- create a ColorPickerComponent
  - inputs: availableColors (string[]) and currentColor (string)
  - outputs: onColorChange (string)
- in the ColorPickerComponent, render a button for each color in availableColors. when the user clicks one of the buttons, emit the color via to the parent component via onColorChange
- In AppComponent, listen to the onColorChange output and update backgroundColor accordingly
- BONUS: in ColorPickerComponent, render the button that matches currentColor slightly differently.
- BONUS (question): what is the ControlValueAccessor interface, and how could it be helpful here?
