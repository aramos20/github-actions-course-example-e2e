# github-actions-course-example-e2e

Repo made for the course I'm taking

CI is the practice of using automation to build and test software every time a developer commits changes to version control. CI helps teams discover issues early in the development process and fix them quickly.

When a workflow produces something other than a log entry, the product is called an artifact

In addition to default environment variables, you can use defined variables as contexts. Contexts and default variables are similar in that they both provide access to environment information, but they have some important differences. While default environment variables can only be used within the runner, context variables can be used at any point within the workflow. For example, context variables allow you to run an if statement to evaluate an expression before the runner is executed

In this example, you're using npm to install the bats software testing package by using the run keyword. You can also run a script as an action. You can store the script in your repository, often done in a .github/scripts/ directory, and then supply the path and shell type using the run keyword.

jobs:
  example-job:
    steps:
      - name: Run build script
        run: ./.github/scripts/build.sh
        shell: bash

Continuous integration (CI) is a practice where developers integrate tested code into a shared branch several times per day. Continuous delivery (CD) is the next phase of continuous integration (CI) where we also make sure to package the code in a release and store it somewhere - preferably, in an artifact repository. Lastly, Continuous deployment (CD) takes continuous delivery (CD) to the next level by directly deploying our releases to the world.

Inputs are the parameters that allow you to specify data that the action expects to use during its runtime. GitHub stores these input parameters as environment variables.

Outputs are the parameters that allow you to declare data
