## Home page
Click "Panel sterowania" to open control pannel site.
![home](https://github.com/kcha01/Data_archiving_S7-1200PLC_WebPage_OPCServer/blob/main/Screenshots/index.PNG?raw=true)

![control](https://github.com/kcha01/Data_archiving_S7-1200PLC_WebPage_OPCServer/blob/main/Screenshots/control_pannel.png?raw=true)

## Number of impulses
This variable is programmed in JavaScript. Script takes number from other file - impulsy.htm. In this manner, value is constantly updated without page reloading.

impulsy.htm file communicates using AWP command.
![impulsy.htm](https://github.com/kcha01/Data_archiving_S7-1200PLC_WebPage_OPCServer/blob/main/Screenshots/impulses.PNG?raw=true)


## Left panel (pace control)

| Button              | Description                |
| :------------------ | :------------------------- |
| `Start`             | Sets base pace for engine  |
| `Stop`              | Stops engine               |
| `Zwiększ prędkość`  | Increases speed by 500     |
| `Zmniejsz prędkość` | Reduces speed by 500       |

## Right panel (alarm)

| Button                 | Description                |
| :--------------------- | :------------------------- |
| `Wykrycie awarii`      | Starts alarm, stops engine |
| `Awaria naprawiona`    | Stops alarm                |
| `Potwierdzenie awarii` | Confirms alarm             |

To communicate with PLC, these buttons are programmed with AWP commands. They work in SET/RESET mode. Reset operations are handled by PLC programme (except "Wykrycie awarii" and "Awaria naprawiona"). 
![AWP](https://github.com/kcha01/Data_archiving_S7-1200PLC_WebPage_OPCServer/blob/main/Screenshots/awp.PNG?raw=true)
![Button](https://github.com/kcha01/Data_archiving_S7-1200PLC_WebPage_OPCServer/blob/main/Screenshots/buttons.PNG?raw=true)

