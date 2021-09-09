#  Kseniya Klimova 
![Image](images/IMG_6745.jpg)

- - -

## **WEB-DEVELOPER** 
                        
  ### *Contacts:* 
        tel: +7937 257 86 51
        e-mail: ksuoxy773@gmail.com    
        

- - -
        
### Information about me 

- - -
 My name is Kseniya. 
* I'm a web-developer. 
* I want to emprove myself in programming. 
* I'm very interested in front-end. 
* I'm keen on creating sites. 

``Also I'm very interested in learning new knowledge.
 Education for me is a new opportunity 
 to get more qualified developer and to get more expierince.
  I'm not afraid of some troubles in my work becase they help me to know much more about web-development. I'm  good at hard-working, I'm team-player  and I'm disciplined so it helps me to do projects on time.``


- - -

#### Skills

1. HTML
2. CSS
3. SASS
4. GIT
5. WEBPACK
6. JAVASCRIPT
7. BEM
8. REACT

- - -
### Code extract
````
const wsUrl =  'wss://echo.websocket.org/';
function pageLoaded() {
  const informationOutput = document.querySelector('.information_output');
  const messageOutput = document.querySelector('.message_output');
  const input = document.querySelector('input');
  const button = document.querySelector('.btn');
  const buttonGeoloc = document.querySelector('.geolocation_btn');
  const output = document.getElementById('output')
const websocket = new WebSocket(wsUrl);
  websocket.onopen = () => {
    informationOutput.innerText = 'Соединение установлено';
  }
  websocket.onmessage = (event) => {
    writeToScreen(`<span style=' color: blue;'> Response ${event.data} </span> `)
}
   websocket.onerror = () => {
      informationOutput.innerText = 'При передаче данных произошла ошибка';
   }
  button.addEventListener('click', sendMessage);
  function sendMessage() {
    if (!input.value) return;
    websocket.send(input.value);
    writeToScreen(input.value);
    input.value === '';
}
  function writeToScreen(message) {
   let pre = document.createElement('p');
   pre.style.wordWrap = "break-word";
   pre.innerHTML = message;
   messageOutput.appendChild(pre);
 }
buttonGeoloc.addEventListener('click',getLocation);
  function getLocation() {
    if ('geolocation' in navigator) {
      navigator.geolocation.getCurrentPosition(locationSuccess, locationError)
    } else {
      writeOutput ('Ваш браузер не поддерживает геолокацию')
    }
  }
  function locationSuccess(data) {
    let link = ` https://yandex.ru/maps/?pt=${data.coords.longitude},${data.coords.latitude}&z=18&l=map`;
  
    writeToScreen (`<a href="${link}" target="_blank">Вы находитесь здесь</a>`);
  }
  function locationError() {
     writeOutput('Произошла ошибка');
  }
  function writeOutput(message) {
    output.innerHTML = `<p>${message}</p>`;
}
}
document.addEventListener('DOMContentLoaded', pageLoaded);
````
- - -
#### My projects
1. [This is landing page "Wildlife"](https://ksy336-wildlife.netlify.app/)
2. [Fill the form](https://codepen.io/ksuoxy/pen/abBbNqP)
3. [Get the link of your GEOLOCATION](https://codepen.io/ksuoxy/pen/wvzKxMQ)
4. [Creation of Websocket connection/Chat](https://codepen.io/ksuoxy/pen/NWRGjby)
5. [Weather forecast](https://codepen.io/ksuoxy/pen/QWKwrwg)

- - -
### Work Experience
* RSSchool (2021)
* Skillfactory (2020-2021)

- - -
### Education 
* RSSchool (2021)
* Skillfactory (2020-2021)
* CS50 (2020)
* Saratov State Technical University - "Manager in social cultural service and tourism" (2010-2015)
*  Saratov State Technical University - "Translator in professional communication" (2010-2015)

- - -
### Languages
```
English: Intermediate level.
I worked as a English teacher for very beginners and for kids at Nova School of English. (2015)
I get a diploma "Translator in professional communication" from SSTU university.(2015)

```


