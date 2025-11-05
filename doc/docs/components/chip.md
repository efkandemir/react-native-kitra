---
sidebar_position: 7
---

# Chip
The **Chips** can be used to display entities in small blocks.

### Import

```js
import { Chip } from '@tra-tech/react-native-kitra';
```

### Usage

```js
import { Chip } from '@tra-tech/react-native-kitra';
import { View } from 'react-native';

const App = () => (
<View style={{ flex: 1, alignItems: 'center', justifyContent: 'center' }}>
  <Chip
    label="Small"
    size="large"
    onChange={e => console.log(e)}
    left={(isSelected) => (
      <Icon
        name="star"
         type="material-community" 
        color={isSelected ? 'gold' : 'gray'}
        size={18}
      />
    )}
    right={(isSelected) => (
      <Icon
        name="check"
        type="material-community" 
        color={isSelected ? 'green' : 'gray'}
        size={18}
      />
    )}
  />
</View>
);

export default App;
```

### Props

| Prop name    | Type                                                                                                           | Required | Description                                                                 |
|--------------|----------------------------------------------------------------------------------------------------------------|----------|-----------------------------------------------------------------------------|
| label        | ``string``                                                                                                     | No       | Text of chip.                                                               |
| value        | ``boolean``                                                                                                     | No       | Status of chip.                  Default value: ``'false'``                                             |
| left         | [``(isSelected?: boolean) => React.ReactNode``](https://reactnative.dev/docs/react-node)                       | No       | Function that returns an element to render on the **left** side of the chip label. Receives the chip’s selected state as a parameter. |
| right        | [``(isSelected?: boolean) => React.ReactNode``](https://reactnative.dev/docs/react-node)                      | No       | Function that returns an element to render on the **right** side of the chip label. Receives the chip’s selected state as a parameter. |
| labelStyle        | [``StyleProp<TextStyle>``](https://reactnative.dev/docs/text-style-props)                                      | No       | Additional styles to apply to the chip.                                     |
| style        | [``StyleProp<ViewStyle>``](https://reactnative.dev/docs/view-style-props)                                      | No       | Additional styles to apply to the label.                                     |                                                     |
| size         | <code> 'small' \| 'medium' \| 'large'</code>                                                                               | No       | The size of the chip. Default value: ``'small'``                              |
| onChange     | ``(event:boolean)=> void``                                                                                     | No      | Returns whether the chip is selected.                                       |
| disabled      | ``boolean ``                                                                                                   | No       | If true the user won't be able to toggle the chip. Default value: ``false`` |
| theme        | ``UITheme ``                                                                                                   | No       | The theme to use for the component.                                      |
| typography   | ``UITypography``                                                                                               | No       | The typography to use for the component.                                 |
