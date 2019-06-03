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

## Usage

```
import RNTimer from "react-native-counter-timer";

const timer = {
  id: 1,
  name: 'DF',
  restTimeHours: 0,
  restTimeMinutes: 0,
  restTimeSeconds: 7,
  activiTimeHours: 0,
  activeTimeMinutes: 0,
  activeTimeSeconds: 8,
  sets: 7,
  createdDate: null,
  modifiedDate: null
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
| `controllerButtons`                              ||  array | ['RESET', 'PRIMARY_ACTION', 'SKIP'] |
| `controllerPosition`                             || String | 'BOTTOM'|
| `controlsWrapperStyle`                           || Object | {flexDirection: 'row',justifyContent: 'space-around',paddingBottom: 10,paddingTop: 10,}|
| `controllerResetText`                            || String | 'RESET'|
| `controllerResetButtonTextStyle`                 || Object | {color: '#0086C6',fontSize: 16}|
| `controllerResetButtonStyle`                     || Object | {paddingTop: 10,alignItems: 'center',flex: 1}| 
| `controllerDisabledResetButtonTextStyle`         || Object | null |
| `controllerDisabledResetButtonStyle`             || Object | null |
| `controllerSkipButtonText`                       || String | 'SKIP'|
| `controllerSkipButtonStyle`                      || Object | {paddingTop: 10,alignItems: 'center',flex: 1,}|
| `controllerDisabledSkipButtonTextStyle`          || Object | null |
| `controllerDisabledSkipButtonStyle`              || Object | null |
| `controllerMainPrimaryActionButtonStyle`         || Object | null |
| `controllerMainPrimaryActionDisabledButtonStyle` || Object | null |
| `controllerSecondPrimaryActionButtonStyle`       || Object | null |

### Progress

| Props | Description |Type | Default Values |
|------------|-------|--------|----------------|
| `progressAnimation`       | If the circle should animate | bool | true|
| `progressBorderWidth`     || Number | 0 |
| `progressDirection`       | Direction of the circle clockwise or counter-clockwise | String | 'clockwise'|
| `progressStyle`           || Object | {alignItems: 'center',justifyContent: 'center',} |
| `progressThickness`       |Thickness of the circle.| Number | 4 |
| `progressVisible`         | Whether or not to visible progress bar | bool |true |
| `progressSize`            |Diameter of the circle | Number | 140  |
| `progressWrapper`         | Override the style of progress circle wrapper| Object | { paddingTop: 30} |
| `progressPrimaryStatusColor` | Progress color when timer in primary status| Object ||
| `progressSecondaryStatusColor` | Progress color when timer in secondary status| Object ||

### Counter

| Props | Description | Type | Default Values |
|------------|--------|-------|----------------|
| `counterTimer` || array | ['HOURS', 'MINUITES', 'SECONDS'] |
| `counterTexts` || array | ['MAX_TIME', 'TIMER', 'SET'] } |
| `counterSetSeperatorText` || String | '/' |
| `counterSetText`          || String | 'Set' |
| `counterSetTextWrapperStyle` || Object | {fontSize: 20, color: 'black'} |
| `counterTimerDefaultStatusText` || String | 'Default' |
| `counterTimerPrimaryStatusText` || String | 'primary' |
| `counterTimerSecondaryStatusText` || String | 'secondary' |


### Gradient Color
| Props | Description | Type | Default Values |
|------------|--------| -------|----------------|
| `gradientColorsDefault` || Object ||
| `gradientColorsRepsActive` || Object ||
| `gradientColorsRestActive` || Object ||

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
