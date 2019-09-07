# react-native-wheel-of-fortune
Wheel of fortune component for React Native

![React Native Wheel Of Fortune](https://github.com/eftalyurtseven/react-native-wheel-of-fortune/raw/master/assets/images/RNWheelOfFortune.gif "React Native Wheel Of Fortune")

![React Native Wheel Of Fortune](https://github.com/eftalyurtseven/react-native-wheel-of-fortune/raw/master/assets/images/demo.png "React Native Wheel Of Fortune")


## Installation

Use the package manager npm and yarn to install react-native-wheel-of-fortune.

```bash
yarn add react-native-wheel-of-fortune
# or using npm
npm i react-native-wheel-of-fortune --save
```

## Dependencies
WheelofFortune is dependent on [react-native-svg](https://github.com/react-native-community/react-native-svg) and [D3-shape](https://github.com/d3/d3-shape) plugins.

## Import

```js
import WheelOfFortune from 'react-native-wheel-of-fortune'
```

## Properties
Property | Type | Default | Desc
--- | --- | --- | ---
rewards *(required)* | `Array` | - | Set Rewards 
winner | `Number` | random | Set winner index
colors | `Array` | Default Colors | Segment background colors
duration *(ms)* | `Number` | 10000 | Completion time  (ms)
getWinner *(required)* | `callback(value,index)` | - | Winner value and index callback function
backgroundColor | `String` | #FFFFFF | Wheel background color
borderWidth | `Number` | 2 | Wheel border width
borderColor | `String` | #FFFFFF | Wheel border color
textColor | `String` | #FFFFFF | Rewards text color
knobSize | `Number` | 20 | Knoob size
knoobSource | `Path` | knoob.png | Knoob source
playButton | `render()` | example | Render method for tap to play button

## Usage
```js
<WheelOfFortune
    rewards={[1, 2, 3, 4, 5, 6, 7, 8, 9]}
    knobSize={20}
    borderWidth={3}
    borderColor={"#FFF"}
    winner={3}
    backgroundColor={"#c0392b"}
    getWinner={(value, index) => this.setState({ winnerValue: value, winnerIndex: index })}
/>        
```
For more information and test go to [/Example](https://github.com/eftalyurtseven/react-native-wheel-of-fortune/tree/master/Example) folder.



## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.


## License
[MIT](https://choosealicense.com/licenses/mit/)