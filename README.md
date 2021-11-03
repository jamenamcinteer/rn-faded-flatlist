# rn-faded-scrollview

A simple and customisable React Native component that allows you to add fade effect in FlatList at both ends. Based on [rn-faded-scrollview](https://github.com/mak12/rn-faded-scrollview).

|     Vertical Scroll      |     Horizontal Scroll      |
| :----------------------: | :------------------------: |
| ![](assets/vertical.gif) | ![](assets/horizontal.gif) |

## Installation

This library relies on [react-native-linear-gradient](https://github.com/react-native-community/react-native-linear-gradient). Follow setup instructions of linear gradient.

And now finally run in your project directory.

`npm install rn-faded-flatlist`

OR

`yarn add rn-faded-flatlist`

## Documentation

This library accepts all the props of [FlatList](https://reactnative.dev/docs/flatlist) and some additional props.

### Props

| Name            | Description                                                                         | Default                                                                               | Type     |
| --------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | -------- |
| allowStartFade  | Add fade at the start of ScrollView                                                 | false                                                                                 | Boolean  |
| allowEndFade    | Add fade at the end of ScrollView                                                   | true                                                                                  | Boolean  |
| fadeSize        | Fade size i.e( width incase of horizontal and height incase of vertical ScrollView) | 20                                                                                    | Number   |
| fadeColors      | Colors for fade effect                                                              | ['rgba(229, 229, 229, 0.18)', 'rgba(206, 201, 201, 0.6)', 'rgba(206, 201, 201, 0.9)'] | Array    |
| scrollThreshold | Threshold to control fade hide/show when it reaches start or end                    | 10                                                                                    | Number   |
| allowDivider    | Allow divider at fade end.                                                          | false                                                                                 | Boolean. |
| isRtl           | For RTL Layouts                                                                     | false                                                                                 | Boolean. |

### Styling

For styling pass these props.

`containerStyle`, `startFadeStyle`, `endFadeStyle` and `dividerStyle`.

### Events

| Name           | Callback param | Description                         |
| -------------- | -------------- | ----------------------------------- |
| isCloseToEnd   | Boolean        | if scroll is close to end or not.   |
| isCloseToStart | Boolean        | if scroll is close to start or not. |
