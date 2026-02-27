    ___    __        __              ____        __   _ __       ______      __      __       __         
   /   |  / /_  ____/ /_  _______   / __ \____ _/ /__(_) /_     /_  __/___ _/ /_  __/ /______/ /__  _____
  / /| | / __ \/ __  / / / / ___/  / /_/ / __ `/ //_/ / __ \     / / / __ `/ / / / / //_/ __  / _ \/ ___/
 / ___ |/ /_/ / /_/ / /_/ / /     / _, _/ /_/ / ,&lt; / / /_/ /    / / / /_/ / / /_/ / ,&lt; / /_/ /  __/ /    
/_/  |_/_.___/\__,_/\__,_/_/     /_/ |_|\__,_/_/|_/_/_.___/    /_/  \__,_/_/\__,_/_/|_|\__,_/\___/_/     
                                                                                                     

```js

import SoftwareDeveloper from 'rakib';

class Bio extends SoftwareDeveloper {
  name     = 'Abdur Rakib Talukder';
  title    = 'Software Developer';
  location = 'Bangladesh';
  mindset  = 'No means next opportunity — keep moving.';
}

class Skills extends SoftwareDeveloper {
  frontend = ['HTML', 'CSS', 'JavaScript'];
  backend  = ['Python', 'PHP', 'Java', 'Kotlin'];
  tools    = ['Git', 'VS Code'];
}

class Mission extends SoftwareDeveloper {
  build() {
    return 'Create clean and useful applications.';
  }

  improve() {
    return 'Learn something new every day.';
  }
}

export default new Bio();
```
