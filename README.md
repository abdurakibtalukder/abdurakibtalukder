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
