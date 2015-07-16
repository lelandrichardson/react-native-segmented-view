# react-native-segmented-view
Segmented View for React Native (with animation)


## Demo

![demo](http://media.giphy.com/media/3oEduLBXWcHSxdN8UE/giphy.gif)

![stretch demo](http://media.giphy.com/media/3oEdv2mvoLWdWmxeik/giphy.gif)


## Example

    <SegmentedView
        titles={["First", "Second", "Third"]}
        index={this.state.index}
        stretch
        onPress={index => this.setState({ index })}
    />


## API (props)

- `titles`: (array) => an array of renderables, or arbitrary data if you specify a `renderTitle` function
- `index`: (number) => the index of the selected title
- `stretch`: (bool) => whether or not the titles fill in the space inbetween each other
- `onPress`: (function(index:number)) => event when a title is tapped, with the index of the title passed in
- `renderTitle`: (function(title: any, index:number)) => if specified, this function will be called for each
- `duration`: (number) => the length (in ms) of the animation of the bar from one title to the other when it gets selected
- `onTransitionStart`: (function) => called when a transition animation starts
- `onTransitionEnd`: (function) => called when a transition animation ends
- `barColor`: (string) => the color of the highlight bar
- `barPosition`: (string) => the position of the highlight bar.
- `underlayColor`: (string) => the underlay color of a title block
- `selectedTitleStyle`: (object) => the style of the selected title block
- `titleStyle`: (object) => the style of a normal (unselected) title block
