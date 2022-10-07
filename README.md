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
