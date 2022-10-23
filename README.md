# Corean
## _Collaborative Refactoring Annotations_

Corean is a library for managing the sharing of responsibility for  refactoring operations.

The first version supports the following refactoring operations:
- Move Method
- Extract Method
- Move Method + Extract Method
- Configurable method refactoring
- Configurable code refactoring

## Annotations

- @MovableMethod (for move method operation)
- @ExtractableCode with pseudo annotations: /*@ExtractableBegin*/ and /*@ExtractableEnd*/ (for extract method operation)
- @MovableCode with pseudo annotations: /*@MovableBegin*/ and /*@MovableEnd*/ (for a series of move method and extract method)
- @MethodRefactorability (for configurable method refactoring)
- @CodeRefactorability (for configurable code refactoring)

## Deployment
In order to add [Corean] library to _intellij_ without source control you need to do the following steps:

Right click -> open _module settings_
 
![image](https://user-images.githubusercontent.com/107777285/183267037-20fcc8e2-60b2-4e54-9c3a-77bd3d8a392d.png)

![image](https://user-images.githubusercontent.com/107777285/183267098-f82c9636-fb9d-4e7b-b4a9-911a67c9be29.png)

_File_ -> _settings_

![image](https://user-images.githubusercontent.com/107777285/183267164-dc7a8fc2-ebb8-4658-ae70-9db0a7510b40.png)

In order to add Corean library to _intellij_ with _Maven_ you need to add:

![image](https://user-images.githubusercontent.com/107777285/183267333-85b22991-1761-4031-bc31-1f86a0aa2118.png)

## Usage notes:
-	In the project file structure, the src folder should be in one of out's/target's parent folders.
-	When using @RefactorableMethod or @RefactorableCode annotations, the configuration file ([refactorability_configuration.json]) should be located in the same folder as the project's src folder.

[Corean]: <https://github.com/refactorability/Collaborative-Refactoring-Annotations/blob/main/collaborative-refactoring-annotations-0.0.1.jar> 
[refactorability_configuration.json]: <https://github.com/refactorability/Collaborative-Refactoring-Annotations> 
