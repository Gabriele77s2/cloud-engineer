# Jenkins

1. **Jenkins**: Jenkins is an open-source automation server used for building, deploying, and automating software development pipelines.

2. **Pipeline**: A Jenkins Pipeline is a set of automated steps that define a software development process, including building, testing, and deploying code.

3. **Job**: A job in Jenkins is a single task or unit of work within a build process. It can include actions like compiling code, running tests, or deploying applications.

4. **Node**: A node in Jenkins is a machine that is part of the Jenkins build environment. Nodes can be either the master (main Jenkins server) or agents (slave machines used for parallel builds).

5. **Plugin**: Jenkins plugins are extensions that add functionality to Jenkins. They allow you to integrate Jenkins with other tools, such as version control systems or cloud services.

6. **SCM (Source Code Management)**: SCM plugins in Jenkins enable integration with version control systems like Git, SVN, and Mercurial, allowing Jenkins to fetch and manage source code.

7. **Build**: A build in Jenkins refers to the process of compiling, assembling, and packaging code to create a software artifact.

8. **Artifact**: An artifact is the result of a build process, such as a compiled executable, library, or deployment package.

9. **Freestyle Project**: A type of Jenkins job that allows users to configure build steps and post-build actions using a graphical interface.

10. **Declarative Pipeline**: A type of Jenkins Pipeline that uses a simplified, structured syntax for defining pipelines.

11. **Scripted Pipeline**: A type of Jenkins Pipeline that allows users to write custom scripts using the Groovy scripting language to define complex build processes.

12. **Executor**: An executor in Jenkins represents a slot for running a build or a job. It can be associated with a node, and the number of executors determines how many jobs can run in parallel.

13. **Artifact Repository**: A location where Jenkins can store and retrieve build artifacts for use in subsequent stages or jobs.

14. **CI/CD**: Continuous Integration (CI) and Continuous Deployment (CD) are software development practices facilitated by Jenkins, where code changes are automatically built, tested, and deployed to production.

15. **Parameter**: A parameter in Jenkins allows users to input values when triggering a build or job, making builds more flexible and customizable.

16. **Workspace**: The workspace in Jenkins is a directory on a node where a build or job is executed. It contains the source code, build artifacts, and other files needed for the job.

17. **SCM Polling**: A feature that allows Jenkins to periodically check a version control system for changes and trigger builds automatically when new commits are detected.

18. **Artifact Retention Policy**: Rules defined in Jenkins to specify how long build artifacts should be kept before they are automatically deleted to save disk space.

19. **Blue Ocean**: A Jenkins plugin and user interface that provides a modern, visual way to create and manage pipelines.

20. **Groovy**: The scripting language used for writing custom scripts in Jenkins, especially in Scripted Pipelines.

21. **Trigger**: A trigger is an event or condition that initiates the execution of a Jenkins job or build. Common triggers include code commits, scheduled times, or manual initiation.

22. **Master-Slave Configuration**: Also known as the Jenkins master-agent setup, this configuration involves a central Jenkins master server that distributes build and deployment tasks to multiple agent nodes for parallel execution.

23. **Artifact Promotion**: The process of moving or promoting artifacts (such as binaries or deployment packages) through different stages of the software delivery pipeline, typically from development to testing and production.

24. **Workspace Cleanup**: Jenkins can be configured to automatically clean up workspace directories after a build or job is completed to free up disk space.

25. **Security Realm**: Jenkins provides various security realms for user authentication, including LDAP, Active Directory, and built-in user databases, to control access to Jenkins resources.

26. **Freestyle Project**: A type of Jenkins job that allows users to configure build steps and post-build actions using a graphical interface.

27. **Secrets Management**: Jenkins provides plugins and features for securely managing sensitive information such as API keys, passwords, and SSH keys used in build and deployment processes.

28. **Agent Label**: In a master-agent (or master-slave) configuration, agent labels are used to assign jobs to specific agent nodes based on predefined labels, ensuring that jobs run on suitable nodes.

29. **JUnit**: A popular testing framework that integrates with Jenkins, allowing the reporting of test results, test trends, and the identification of failing tests.

30. **Parameterized Builds**: Jenkins supports parameterized builds, enabling users to customize build configurations by providing input parameters when triggering a job.

31. **Pipeline as Code**: The practice of defining Jenkins Pipelines using code (typically in a version-controlled repository) rather than configuring them through the Jenkins web interface.

32. **Docker Integration**: Jenkins can integrate with Docker to build and run containers, making it easier to manage dependencies and build environments.

33. **Matrix Project**: A Jenkins project type that allows for the parallel execution of a job across multiple axes of parameters, making it useful for testing across various configurations.

34. **Job DSL (Domain Specific Language)**: A plugin that allows users to define Jenkins job configurations programmatically using a Groovy-based DSL, facilitating the management of large numbers of jobs.

35. **GitHub Integration**: Jenkins can integrate with GitHub to trigger builds and deployments based on code changes, pull requests, and other GitHub events.

36. **Jenkinsfile**: A file used in Jenkins Pipelines to define the entire pipeline as code, including stages, steps, and configuration, often stored in the version control repository alongside the source code.

37. **JUnit Plugin**: A Jenkins plugin that parses JUnit XML test result files and provides detailed test reports within Jenkins.

38. **SSH Agent Plugin**: A Jenkins plugin that allows the temporary use of SSH keys during a build or deployment process, useful for securely accessing remote servers or repositories.

39. **SonarQube**: An integration with Jenkins for performing code quality and static analysis checks on code as part of the build process.

40. **Jenkins Configuration as Code (JCasC)**: A plugin and approach that allows administrators to define and configure Jenkins settings and jobs using YAML or other configuration files, promoting infrastructure as code practices.

## Jenkins Commands

1. **Jenkins CLI (Command Line Interface)**: Jenkins provides a CLI tool that allows you to interact with Jenkins from the command line. You can download the Jenkins CLI JAR file from the Jenkins server and use it to perform various tasks, such as triggering builds, configuring jobs, and managing nodes.

   Example:
   ```bash
   java -jar jenkins-cli.jar -s http://jenkins-server/ help
   ```

2. **Jenkins Job DSL**: The Jenkins Job DSL plugin enables you to define and configure Jenkins jobs programmatically using a Groovy-based DSL. You can use the `jenkins-jobs` command-line tool to generate and update job configurations.

   Example:
   ```bash
   jenkins-jobs update my-job.groovy
   ```

3. **Jenkinsfile**: Jenkins Pipeline can be defined in a Jenkinsfile, which is typically stored in your version control repository. You can use the `jenkinsfile-runner` command-line tool to test Jenkinsfiles locally.

   Example:
   ```bash
   jenkinsfile-runner -w /path/to/workspace -p my-pipeline.groovy
   ```

4. **Jenkins Plugins**: Jenkins plugins often come with their own command-line tools. For example, the Docker Pipeline plugin provides commands for Docker-related operations in pipelines.

   Example:
   ```bash
   docker.build("my-image")
   ```

5. **Curl**: You can use `curl` or similar HTTP client tools to trigger Jenkins builds remotely using the Jenkins REST API. You'll need to authenticate and use appropriate API endpoints.

   Example:
   ```bash
   curl -X POST -u username:password http://jenkins-server/job/my-job/build
   ```

6. **Jenkins Configuration as Code (JCasC)**: If you're using JCasC to configure Jenkins, you typically define your configuration in a YAML file and apply it to Jenkins using the `java -jar jenkins.war` command.

   Example:
   ```bash
   java -jar jenkins.war --argumentsRealm.passwd.<username>=<password> --argumentsRealm.roles.<username>=admin --httpPort=8080
   ```

7. **Jenkins SSH Slaves**: If you manage Jenkins agents (slaves) using SSH, you can use SSH commands to start and stop agents on remote machines.

   Example:
   ```bash
   ssh <agent-username>@<agent-hostname> java -jar agent.jar -jnlpUrl http://jenkins-server/computer/my-agent/slave-agent.jnlp
   ```
