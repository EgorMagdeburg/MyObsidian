## Click Counter

```runjs
let count = 0;

function updateCounter() {
    count++;
    counterElement.textContent = `Clicks: ${count}`;
}

const button = document.createElement('button');
button.textContent = 'Click Me!';
button.style.padding = '10px';
button.style.margin = '10px';

const counterElement = document.createElement('p');
counterElement.textContent = 'Clicks: 0';
counterElement.style.fontWeight = 'bold';

button.addEventListener('click', updateCounter);

output.appendChild(button);
output.appendChild(counterElement);
```
