# React Stale Closure Bug
This example demonstrates a common mistake in React's useState hook, leading to a stale closure issue. The bug arises when trying to update state multiple times within a single event handler. The second call to setCount uses the initial value of count, not the updated one. 

## How to Reproduce
1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server. 
4. Click the increment button. Notice that the count does not increment by two each time, exhibiting stale closure.