# React Native: undefined is not an object (evaluating 'state.someProperty')
This repository demonstrates a common React Native error: 'undefined is not an object (evaluating 'state.someProperty')'. This typically happens when you try to access a state variable before it's been properly initialized.  The solution involves careful state management to ensure state values are available before being accessed.

## Problem
The core issue is a race condition. The component renders before the state has had a chance to update to a defined value.  This frequently occurs with asynchronous operations or during the initial render cycle of a component.