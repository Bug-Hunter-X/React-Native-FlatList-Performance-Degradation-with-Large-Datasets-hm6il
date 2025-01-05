# React Native FlatList Performance Issue

This repository demonstrates a common performance issue in React Native's `FlatList` component when dealing with large datasets. The app becomes slow and unresponsive, especially on low-end devices. This example shows the problem and a potential solution using techniques like windowing and virtualization.

## Problem

The provided `FlatListBug.js` shows a `FlatList` rendering a large number of complex components.  This leads to significant performance degradation. Scrolling becomes sluggish, and the app may crash.

## Solution

The `FlatListSolution.js` demonstrates how to optimize the `FlatList` by implementing windowing (rendering only the visible items) and reducing the complexity of the individual item components.  Consider using `React.memo` for component optimization as well.

## How to Reproduce

1. Clone the repository.
2. Run `npm install`
3. Run the app using a simulator or a physical device (try on a device with lower specs for more noticeable issues).