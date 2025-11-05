---
sidebar_position: 15
---

# Progress Bar

The **ProgressBar** component is a visual indicator of a progress. It displays a progress bar with a color that can be customized. The progress bar will animate and fill up based on the progress passed in as a percentage value.

### Import

```js
import { ProgressBar } from '@tra-tech/react-native-kitra';
```
### Usage

```js
import { ProgressBar } from '@tra-tech/react-native-kitra';
import { View, StyleSheet } from 'react-native';

const App = () => (
  <View style={style.container}>
    <ProgressBar progress={25} />
  </View>
);

const style = StyleSheet.create({
  container: { flex: 1, justifyContent: 'center', rowGap: 50 },
});

export default App;
```
### Props

| Prop Name     | Type                | Required | Description |
|---------------|---------------------|----------|-------------|
| progress      | ``number``              | No       | The progress value as a percentage. Default value: ``0`` |
| progressStyle | [``StyleProp<ViewStyle>``](https://reactnative.dev/docs/view-style-props)  | No       |Style object to be applied to the progress bar. |
| barStyle      | [``StyleProp<ViewStyle>``](https://reactnative.dev/docs/view-style-props) | No       | Style object to customize the progress bar container.       |
| theme         | ``UITheme``              | No       | The theme to use for the component. |

