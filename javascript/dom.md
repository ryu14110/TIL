[error 모음]
--20230815 shopping Mall (react)
react-jsx-dev-runtime.development.js:87 Warning: Each child in a list should have a unique "key" prop.

Check the render method of `Navbar`. See https://reactjs.org/link/warning-keys for more information.
    at li
    at Navbar (http://localhost:3000/static/js/bundle.js:166:81)
    at div
    at App (http://localhost:3000/static/js/bundle.js:41:90)
    at Router (http://localhost:3000/static/js/bundle.js:43575:15)
    at BrowserRouter (http://localhost:3000/static/js/bundle.js:41676:5)
-->
<ul>
  {items.map((item, index) => (
    <li key={item.id}>{item.name}</li>
  ))}
</ul>
