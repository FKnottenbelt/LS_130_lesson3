# LS_130 lesson 3: setting up a project

We need a seperate git repro for this lesson (todolist_project structure)


Typically, ruby projects have a strict organization. Specifically,
developers expect to find test code in a `test` directory, and Ruby source
files in the `lib` directory.

Make sure to setup the require_relative path in you test correctly

todolist_project
├── README.md
├── lib
│   └── todolist_project.rb
└── test
    └── todolist_project_test.rb
    
    
There are many other directories that you may need. For instance, 
web-based programs generally require "assets" like images, JavaScript,
and CSS (stylesheets) -- these often reside in an `assets` directory
with a `subdirectory` for each file type: `images`, `javascript`, and
`stylesheets`. 

HTML "template" files usually reside in a `views` directory. 