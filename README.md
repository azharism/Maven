# Maven

Maven build lifecycle goes through a set of stages, they are called build phases. For example, the default lifecycle is made up of the following phases.

validate
compile
test
package
verify
install
deploy
=========================================================================================================================================
Each of these build lifecycles is defined by a different list of build phases, wherein a build phase represents a stage in the lifecycle.

For example, the default lifecycle comprises of the following phases (for a complete list of the lifecycle phases, refer to the Lifecycle Reference):
=========================================================================================================================================================================

1.validate – validate the project is correct and all necessary information is available
2.compile – compile the source code of the project
3.test – test the compiled source code using a suitable unit testing framework. These tests should not require the code be packaged or deployed
4.package – take the compiled code and package it in its distributable format, such as a JAR or war.
5.verify – run any checks on results of integration tests to ensure quality criteria are met
6.install – install the package into the local repository, for use as a dependency in other projects locally. .m2 (folder)
7.deploy – done in the build environment, copies the final package to the remote repository for sharing with other developers and projects on artifact repository like nexus.
