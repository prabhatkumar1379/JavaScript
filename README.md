# JavaScript
<h3>JavaScript CallBack</h3>

**A callback is a function passed as an argument to another function**, which is then invoked after the main function completes its task. Callbacks are commonly used for handling asynchronous operations, ensuring specific code runs after an action is finished, like fetching data or responding to user actions.

```javascript
function fetchData(url, callback) {
  setTimeout(() => {
    console.log("Data fetched from", url);
    callback("Sample Data");
  }, 1000);
}

function handleData(data) {
  console.log("Handling the data:", data);
}

fetchData("https://example.com", handleData);
