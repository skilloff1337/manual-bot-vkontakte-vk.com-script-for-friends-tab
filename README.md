# Semi-automatic bot via browser console
**EN:**
To use scripts, you will need to launch a browser with a built-in console (Tested on Google Chrome), open the desired section on the vk.com website, press the ```F12``` key, open the **Console** tab, and paste the copied code under the desired task.

**RU:**
Для использование скриптов, потребуется запустить браузер со встроенной консолью (Проверено на Google Chrome), открыть нужнный раздел на сайте vk.com, нажать на клавишу ```F12```, открыть вкладку **Console**, и вставить скопированный код под нужную задачу.

## Accepting all friend requests (Принятие все заявки в друзья)
```
var buttons = document.getElementsByTagName('button');
for(var i = 0; i < buttons.length; i++)
{
  var thisButton = buttons[i];
  if(thisButton.id.includes("accept_request"))
    thisButton.click()
}
```
