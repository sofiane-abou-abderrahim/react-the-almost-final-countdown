# Refs & Portals

## Advanced DOM Access & Value Management

# Tasks

- Accessing DOM Elements with Refs
- Managing Values with Refs
- Exposing API Functions from Components
- Detaching DOM Rendering from JSX Structure with Portals

# Steps

## 0. Module Introduction & Starting Project

1. run `npm install`
2. run `npm run dev`
3. create `README.md`

## 1. Repetition: Managing User Input with State (Two-Way-Binding)

1. use `useState()` and two-way-binding in `Player.jsx`

## 2. Introducing Refs: Connecting & Accessing HTML Elements via Refs

1. replace `useState()` with `useRef()` in `Player.jsx` because it is more convenient

## 3. Manipulating the DOM via Refs

1. use `useRef()` to clear the input in `Player.jsx`

## 4. Adding Challenges to the Demo Project

1. create `TimerChallenge.jsx` component
2. output `<TimerChallenge />` components in `App.jsx`

## 5. Setting Timers & Managing State

1. use `useState()` to set a timer in `TimerChallenge.jsx`
2. render UI dynamically

## 6. Using Refs for More Than "DOM Element Connections"

1. use `useRef()` in `TimerChallenge.jsx` to store the `timer` value without resetting it when the component is reexecuted

## 7. Adding a Modal Component

1. create `ResultModal.jsx` component
2. output the `<ResultModal />` component in `TimerChallenge.jsx`

## 8. Forwarding Refs to Custom Components

1. reach out the dialog in `ResultModal` from `TimerChallenge.jsx` with help of `useRef()`
2. forward the ref defined in `TimerChallenge.jsx` to the dialog element in `ResultModal.jsx` with help of the `forwardRef` function
3. use this dialog in `TimerChallenge.jsx`

## 9. Exposing Component APIs via the useImperativeHandle Hook

1. detach the `TimerChallenge.jsx` component from the `dialog` element from the ``ResultModal.jsx` component with help of `useImperativeHandle()`

## 10. More Examples: When To Use Refs & State

1. measure how much time is left on an ongoing basis with `setInterval()` instead of `setTimeout` in `TimerChallenge.jsx`
2. use `clearInterval()` instead of `clearTimeout()`

## 11. Sharing State Across Components

1. forward the correct information to the modal by replacing the `result` prop with the `remainingTime` prop
2. use the `remainingTime` prop to calculate the score or find out if the user lost in `ResultModal.jsx`
3. add a `handleReset` function to reset the remaining time correctly
4. trigger the `handleReset()` function through a `onReset` prop from `ResultModal.jsx`

## 12. Enhancing the Demo App "Result Modal"

1. calculate the score in `ResultModal.jsx`
2. output the score dynamically

## 13. Closing the Modal via the ESC (Escape) Key

1. add the built-in `onClose` prop to the `<dialog>` element and bind it to the `onReset` prop value
