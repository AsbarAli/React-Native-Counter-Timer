# React Native Counter Timer

## Installation

```
npm i react-native-counter-timer --save 
``` 
or
``` 
yarn add react-native-counter-timer
```

![](https://github.com/AsbarAli/counter/blob/master/src/assets/gif/com2.gif?raw=true)
![](https://github.com/AsbarAli/counter/blob/master/src/assets/gif/03.gif?raw=true)

## Usage - Basic

```
import RNTimer from "react-native-counter-timer";

const timer = {
  restTimeHours: 0,
  restTimeMinutes: 0,
  restTimeSeconds: 7,
  activiTimeHours: 0,
  activeTimeMinutes: 0,
  activeTimeSeconds: 8,
  sets: 7,
 };

 <RNTimer 
  timer={timer}
  controlsWrapperStyle={{
    flexDirection: 'row',
    alignItems: 'center',
    padding: 10}}
  />
```

## Props

### Controller

| Props | Description |  Type | Default Values |
| ------------- |----------- |------------- |----|
| `controllerButtons`   |3 controller buttons and swap the values in the array to change the button order|  array | ['RESET', 'PRIMARY_ACTION', 'SKIP'] |
| `controllerPosition`  | controller position at 'TOP'or 'BOTTOM'| String | 'BOTTOM'|
| `controlsWrapperStyle` | Wrapper style of controller | Object | {flexDirection: 'row',justifyContent: 'space-around',paddingBottom: 10,paddingTop: 10,}|

### Controller - Reset Button
| Props | Description |  Type | Default Values |
| ------------- |----------- |------------- |----|
| `controllerResetText`| Reset button text | String | 'RESET'|
| `controllerResetButtonTextStyle` |Reset button text style| Object | {color: '#0086C6',fontSize: 16}|
| `controllerResetButtonStyle` |Reset button style| Object | {paddingTop: 10,alignItems: 'center',flex: 1}| 
| `controllerDisabledResetButtonTextStyle` | Reset button text style when button is disable| Object | null |
| `controllerDisabledResetButtonStyle` | Reset button style when when button is disable| Object | null |
| `controllerResetButtonElement`| React native element inside the reset button | Object | null |

### Controller - Skip Button
| Props | Description |  Type | Default Values |
| ------------- |----------- |------------- |----|
| `controllerSkipButtonText`  | Skip Button text| String | 'SKIP'|
| `controllerSkipButtonStyle` |Skip button text style | Object | {paddingTop: 10,alignItems: 'center',flex: 1,}|
| `controllerDisabledSkipButtonTextStyle` |Skip button text style when button is disabled| Object | null |
| `controllerDisabledSkipButtonStyle` | Skip button style when button is disabled| Object | null |
| `controllerSkipButtonElement`| React native element inside the skip button | Object | null |

### Controller - Action Button (first)
| Props | Description |  Type | Default Values |
| ------------- |----------- |------------- |----|
| `controllerMainPrimaryActionButtonStyle` | Style of main primary button | Object | null |
| `controllerMainPrimaryActionDisabledButtonStyle` | Style of main primary button when disable| Object | null| 
| `controllerMainPrimaryActionButtonElement`| React native element inside primary action button | Object|null|

### Controller - Action Button (Second)
| Props | Description |  Type | Default Values |
| ------------- |----------- |------------- |----|
| `controllerSecondPrimaryActionButtonTextStyle` | Style of second primary action | Object | null |
| `controllerSecondPrimaryActionButtonStyle`  | Style of second primary action button style| Object | null |
| `controllerSecondPrimaryActionButtonElement` | React native element inside second primary action button | Object| null |

### Progress

| Props | Description |Type | Default Values |
|------------|-------|--------|----------------|
| `progressAnimation`       | If the circle should animate | bool | true|
| `progressBorderWidth`     || Number | 0 |
| `progressDirection`       | Direction of the circle clockwise or counter-clockwise | String | 'counter-clockwise'|
| `progressStyle`           | Progress Style | Object | {alignItems: 'center',justifyContent: 'center',} |
| `progressThickness`       |Thickness of the circle.| Number | 4 |
| `progressVisible`         | Whether or not to visible progress bar | bool |true |
| `progressSize`            |Diameter of the circle | Number | 140  |
| `progressWrapper`         | Override the style of progress circle wrapper| Object | { paddingTop: 30} |
| `progressPrimaryStatusColor` | Progress color when timer in primary status| Object | '#31708E' |
| `progressSecondaryStatusColor` | Progress color when timer in secondary status| Object | '#E85A4F'|

### Counter

| Props | Description | Type | Default Values |
|------------|--------|-------|----------------|
| `counterTimer` | Display order of hours, minutes and seconds. swap the value to change the order or remove. Ex: ['SECONDS', 'MINUITES']  | array | ['HOURS', 'MINUITES', 'SECONDS'] |
| `counterTexts` | Display order of max timer, timer and sets. Swap the value in array to change the order or remove | array | ['MAX_TIME', 'TIMER', 'SET'] } |

### Counter - Set
| Props | Description | Type | Default Values |
|------------|--------|-------|----------------|
| `counterSetSeperatorText` | Symbol to seperate between counter set text and number | String | '/' |
| `counterSetText`          | Text of counter set| String | 'Set' |
| `counterSetTextWrapperStyle` | Wrapper style of counter text | Object | {fontSize: 20, color: 'black'} |

### Counter - Status
| Props | Description | Type | Default Values |
|------------|--------|-------|----------------|
| `counterTimerDefaultStatusText` | Counter timer text value before start the timer | String | 'Default' |
| `counterTimerPrimaryStatusText` | Counter timer text value when timer in primary status| String | 'primary' |
| `counterTimerSecondaryStatusText` | Counter timer text value when timer in secondary status| String | 'secondary' |


### Gradient Color
| Props | Description | Type | Default Values |
|------------|--------| -------|----------------|
| `gradientColorsDefault` | Gradient color of timer container before start the timer | Object |'['rgba(255, 255, 255, 0)', 'rgba(255, 255, 255, 0)']'|
| `gradientColorsRepsActive` | Gradient color of timer container when timer is in primary mode | Object |'['rgba(255, 255, 255, 0)', 'rgba(255, 255, 255, 0)']'|
| `gradientColorsRestActive` | Gradient color of timer container when timer is in Secondary mode  | Object |'['rgba(255, 255, 255, 0)', 'rgba(255, 255, 255, 0)']'|

More info - https://github.com/react-native-community/react-native-linear-gradient

### Events

| Props | Description | Default Values |
|------------|---------------|----------------|
| `onActivityCompleted` | Invoke after completed the timer| null |
| `onSecondaryModeEnd`| Invoke when secondary mode end|null |
| `onPrimaryModeStartPressed` | Invoke when press start button in primary mode|null |
| `onSecondaryModePausePressed`| Invoke when press pause button in secondary mode |null |
| `onPrimaryModePausePressed`| Invoke when presss pause button in primary mode | null |
| `onSecondaryModeStartPressed`| Invoke when press start button in secondary mode |null |
| `onSkipPressed`| Invoke when press skip button |null |


License
----

MIT


**Free Software, Hell Yeah!**