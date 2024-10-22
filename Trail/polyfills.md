# Polyfills
* It is the function where we have write a particular function manully to make it work in older browsers. 
* For example, we can use the `map()`
* map() fun was introduced in 2015 so it is not avaliable in older browsers. So we have to write a polyfill for it.

## Importance of polyfills
1.  Cross-browser compaatibility
2.  Improved user experience
3.  Reduced maintenance efforts
4.  progressive enhancement

## Disadvantages
1.  Increased bundle size
2.  Potential performance issues
3.  Overuse of polyfills can lead to code bloat
4.  polyfills can introduce bugs

## Woking of polyfills
1.  Detecting the feature
2.  Providing a fallback implementation

# _Interview que_
we could have rely on third-party libraries that provide polyfills instead of writing our own from scratch? 

_Ans:_ Using a third-party library that provides polyfills can have several disadvantages:

1. _Overhead of Including a Third-Party Library:_ Incorporating an external library increases the overall size of your application, potentially impacting performance.

2. _Potential Conflicts with Other Libraries:_ Third-party libraries may conflict with other libraries in your project, leading to unexpected behavior.
3. _Lack of Control Over the Polyfills:_ When utilizing a library, you may not have full control over how the polyfills are implemented or updated.
4. _Potential Security Risks:_ Relying on external code can introduce vulnerabilities if the library is not properly maintained or audited.
5. _Maintenance and Updates:_ If the library is not actively maintained or updated, you may be  left with outdated polyfills that no longer work as expected.

By coding polyfills from scratch, you can minimize storage usage, maintain greater control over their functionality, and avoid potential conflicts with other libraries.

