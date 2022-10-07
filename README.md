# Learn-react
Notes to learn and revise thr react concepts

## Fragments, Portals and Refs in react
- JSX limitations and fragments
- Getting a cleaner dom with portals
- whar are refs and why we need them

#### JSX Limitations

```
return(
<h1>heading</h1>
<p>paragraph</p>
)
```
> this gives us error because you can't return more than one jsx "root" element
### solutions:
#### - wrap the adjacent elements
```
return(
<div>
  <h1>heading</h1>
  <p>paragraph</p>
 </div>
)
```
> A new problem will arrive "div soup"

#### - wrapper compnent - it wont be rendered on dom but still does the job
#### - fragments - react provides us the build in wrapper component.

### protals 
#### - provides a way to render children into a DOM node that exists outside the heirarchy of the parent components

### refs
#### - used to store the refernce of an element (not a value : for value we use useState hook).
#### - useState is responsible for re-rendering that particular dom element whereas in useRef the dom element will never be re-rendered.
#### - useRef returns object who has single property .current which is initialized to the argument
```
const refContainer = useRef(initialValue);
```
