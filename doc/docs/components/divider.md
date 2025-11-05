---
sidebar_position: 8
---

# Divider
The **Divider**  is a thin, lightweight separator that groups content in lists and page layouts.

### Import

```js
import { Divider } from '@tra-tech/react-native-kitra';
```
### Usage

```js
import { Divider } from '@tra-tech/react-native-kitra';
import { View } from 'react-native';

const App = () => (
  <View style={{ flex: 1, alignItems: 'center', justifyContent: 'center', rowGap: 50 }}>
    <Divider variant="dashed" width={350} />
    <Divider variant="dotted" width={300} />
    <Divider variant="solid" width={200} />
  </View>
);

export default App;
```
### Props

| Prop name  | Type                                                                      | Required | Description                                          |
|------------|---------------------------------------------------------------------------|----------|------------------------------------------------------|
| variant     | <code>'solid' \| 'dotted' \| 'dashed'</code>                             | No       | Style of the divider border. Default value: ``'solid'``                   |
| width      | <code>number \| string</code>                                                                         | No       | Width of divider. Default value: ``'100%'``             |
| borderWidth | ``number``                                                                | No       | Thickness of the divider border. Default value: ``1``                     |
| style      | [``StyleProp<ViewStyle>``](https://reactnative.dev/docs/view-style-props) | No       | Additional styles to apply to the divider.           |
| theme      | ``UITheme ``                                                              | No       | The UI theme to use for the component.               |

