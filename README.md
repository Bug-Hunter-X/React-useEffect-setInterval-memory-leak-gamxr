# React useEffect setInterval memory leak
This repository demonstrates a common error in React components using `setInterval` within the `useEffect` hook, leading to memory leaks. The bug involves the absence of a cleanup function in the `useEffect` hook which prevents the `setInterval` from being properly cancelled when the component unmounts, resulting in a persistent memory leak.  The solution demonstrates the correct usage of the cleanup function to effectively avoid this issue. 