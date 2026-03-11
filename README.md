<br>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/abdurakibtalukder/abdurakibtalukder/refs/heads/main/assets/Asset%206abdurakibtalukder-light.webp" width="70%">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/abdurakibtalukder/abdurakibtalukder/refs/heads/main/assets/Asset%207abdurakibtalukder-dark.webp" width="70%">
    <img alt="logo" src="https://raw.githubusercontent.com/abdurakibtalukder/abdurakibtalukder/refs/heads/main/assets/Asset%207abdurakibtalukder-dark.webp" width="70%">
  </picture>
</p>

<br>

```js
const abdurakibtalukder = {

  name        : 'Abdul Rakib Talukder',
  age         : 15,                             
  location    : 'Bangladesh',
  username    : '@abdurakibtalukder',

  education: {
    school    : 'Ambition Public School, Bhairab',
    degree    : 'Humanities — Arts & ICT',
    field     : 'Software Development',
    status    : `ssc in ${2028}`,         
  },

  career: {
    role      : 'Full Stack Developer',
    stack     : ['JavaScript', 'React', 'Node.js', 'Python'],
    status    : 'busy()',                     
    openTo    : ['collabs', 'open source', 'cool ideas'],
  },

  hobbies     : ['Open Source', 'Planning', 'Cycling', 'Gaming'],

  philosophy  : 'Build clean, useful, and meaningful things.',

  getAge()    { return Date.now() - new Date('2011').getTime(); },
  isAvailable() { return this.career.status !== 'busy()'; },

};
```
