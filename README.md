# React Native Dimensions API - Undefined Dimensions Issue

This repository demonstrates a common issue in React Native development involving the `Dimensions` API. The problem arises when trying to access screen dimensions before they are available, leading to undefined values.

## Problem

The `Dimensions` API doesn't always provide dimensions immediately upon component mount. Accessing `Dimensions.get('window').width` or `Dimensions.get('window').height` before the values are ready results in `undefined`, potentially causing errors or incorrect layout.

## Solution

The solution involves using the `useEffect` hook to access the dimensions after the component has mounted and the values are ready. This ensures the app doesn't crash or render incorrectly due to undefined dimensions.

## Usage

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install the necessary dependencies.
4. Run `npx react-native run-android` or `npx react-native run-ios` to run the application.