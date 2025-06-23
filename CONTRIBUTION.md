HTML code that was used for screenshots before/after

```html
<h1>Main Title</h1>

<div>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
</div>

<h2>Code Snippet</h2>

<code>function hello(name) {
  return `Hello, ${name}!`;
}
</code>

<h3>List Example</h3>

<ol>
  <li>First item <code>with some inline code</code></li>
  <li>Second item</li>
  <li>Third item</li>
</ol>

<h4>Table</h4>

<table>
  <thead>
    <tr>
      <th>Language</th>
      <th>Use Case</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Python</td>
      <td>Data Science</td>
    </tr>
    <tr>
      <td>JavaScript</td>
      <td>Web Development</td>
    </tr>
  </tbody>
</table>

<blockquote>
  “Programs must be written for people to read, and only incidentally for machines to execute.”
</blockquote>
```

Some ChatGPT generated response to test on real-life example

```html
<div><strong>Closures in JavaScript</strong> are functions that "remember" the scope in which they were created, even after that scope has finished executing.</div>

<h3>🔹 Key Concepts (List)</h3>
<ul>
<li>
<div>A <strong>closure</strong> is created when a function is defined inside another function.</div>
</li>
<li>
<div>The inner function has access to:</div>
<ol>
<li>
<div>Its own scope</div>
</li>
<li>
<div>The outer function’s variables</div>
</li>
<li>
<div>Global variables</div>
</li>
</ol>
</li>
<li>
<div>Closures allow <strong>data privacy</strong> and <strong>encapsulation</strong>.</div>
</li>
</ul>

<h3>🔹 Example Code</h3>
<pre><code>function makeCounter() {
  let count = 0;
  return function() {
    count++;
    return count;
  };
}

const counter = makeCounter();
console.log(counter()); // 1
console.log(counter()); // 2
</code></pre>
<blockquote>
<div><code>counter</code> keeps access to <code>count</code> even after <code>makeCounter()</code> has finished.</div>
</blockquote>

<h3>🔹 Closure Access Table</h3>
<table>

<tbody><tr>
<th>Scope Accessed by Inner Function</th>
<th>Example</th>
<th>Accessible?</th>
</tr>


<tr>
<td>Local variable</td>
<td><code>count</code></td>
<td>✅ Yes</td>
</tr>
<tr>
<td>Outer function variable</td>
<td><code>makeCounter</code></td>
<td>✅ Yes</td>
</tr>
<tr>
<td>Global variable</td>
<td><code>console</code></td>
<td>✅ Yes</td>
</tr>
<tr>
<td>Another inner function scope</td>
<td>N/A</td>
<td>❌ No</td>
</tr>

</tbody></table>

<div>Let me know if you want real-world use cases or interview-style questions!</div>
```
