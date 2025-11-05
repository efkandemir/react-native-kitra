---
sidebar_position: 6
---

# CheckBox

The **CheckBox** component is a UI element that allows the user to toggle between two states: checked and unchecked.

### Import

```js  
import { CheckBox } from '@tra-tech/react-native-kitra';
```
### Usage

```js  
import { CheckBox } from '@tra-tech/react-native-kitra';
import { useState } from 'react';
import { View } from 'react-native';

const App = () => {
  const [value, setValue] = useState(false);

  return (
    <View style={{ justifyContent: 'center', flex: 1 }}>
      <CheckBox
        variant="circular"
        style={{ alignSelf: 'center' }}
        value={value}
        onChange={(value) => console.log(value)}
        onPress={() => setValue(prev => !prev)}
      />
    </View>
  );
};

export default App;
```
### Props

| Prop name | Type | Required | Description |
| --- | --- | --- | --- |
| value | `boolean` | No | Determines whether the checkbox is checked or unchecked |
| onChange | `(value: boolean) => void` | No | A callback function that is called when the checkbox is pressed, with the new state value as an argument |
| onPress | `(value: boolean) => void` | No | Called when the checkbox is pressed. Receives the new value as a parameter. |
| style | [``StyleProp<ViewStyle>``](https://reactnative.dev/docs/view-style-props) | No | Additional styles to apply to the checkbox container |
| disabled | `boolean` | No | Determines whether the checkbox is disabled or not |
| variant | `'circular'` \| `'square'` | No | Defines the shape of the checkbox. Default value: `'circular'`. |
| theme | `UITheme` | No | An object containing the color palette used for the checkbox |
| ...TouchableOpacityProps | [``...TouchableOpacityProps``](https://reactnative.dev/docs/touchableopacity#props) | No | Any additional props to be passed to the underlying `TouchableOpacity` component. |

