# LS_130 lesson 3: setting up a project

We need a seperate git repro for this lesson (todolist_project structure)

covers:
- create a repro
- set up directories
- set up the Gemfile
- install new ruby version with rvm
- install bundler
- run bundler
- adding gems
- set up your rakefile
- make your project into a rubygem
  - add directories
  - prepare README.md
  - write documentation
  - prepare gemspec file
  - add gemspec to Gemfile
  - rerun bundler install
  - add Rubygem task to rakefile
  - run rake build

final project structure:
```
todolist_project
├── Gemfile
├── Gemfile.lock
├── lib
│   └── todolist_project.rb
├── pkg
│   └── todolist_project-1.0.0.gem
├── Rakefile
├── README.md
├── test
│   └── todolist_project_test.rb
└── todolist_project.gemspec
```