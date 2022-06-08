# Semi-automatic bot via browser console
**EN:**
To use scripts, you will need to launch a browser with a built-in console (Tested on Google Chrome), open the desired section on the vk.com website, press the ```F12``` key, open the **Console** tab, and paste the copied code under the desired task.

**RU:**
Для использование скриптов, потребуется запустить браузер со встроенной консолью (Проверено на Google Chrome), открыть нужнный раздел на сайте vk.com, нажать на клавишу ```F12```, открыть вкладку **Console**, и вставить скопированный код под нужную задачу.

# Frieds section| Раздел друзья

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

## Delete friends (Удалить друзей)
<br/>EN: To edit the required number of friends, in the script ```var i = 0; i < buttons.length; i++``` buttons.length - you need to change it to your own value.Default - will remove all uploaded friends on the page.
<br/>RU: Что бы отредактировать требуемое количество друзей, в скрипте ```var i = 0; i < buttons.length; i++``` buttons.length - нужно поменять на свое значение. По умолчанию - удалит всех прогруженных друзей на странице.
```
var buttons = document.querySelectorAll(".friends_actions_menu .ui_actions_menu a:nth-child(4)")
for(var i = 0; i < buttons.length; i++)
{
  var thisButton = buttons[i];
    thisButton.click()
}
```

## Delete all outgoing requests (Удалить все исходящие заявки)
```
var buttons = document.getElementsByTagName('button');
for(var i = 0; i < buttons.length; i++)
{
  var thisButton = buttons[i];
  if(thisButton.id.includes("deny_request"))
    thisButton.click()
}
```

## Send a request in the "Find friends" section (Отправить запрос в разделе "Поиск друзей")
**Important | Важно** 
<br/>EN: Add no more than 50 friends. To edit the required number of friends, in the script ```var i = 0; i < 50; i++``` 50 - you need to change it to your own value.
<br/>RU: Добавлять не более 50 друзей. Что бы отредактировать требуемое количество друзей, в скрипте ```var i = 0; i < 50; i++``` 50 - нужно поменять на свое значение.
```
var buttons = document.getElementsByClassName('friends_find_user_add');
for(var i = 0; i < 50; i++)
{
  var thisButton = buttons[i];
    thisButton.click()
}
```
